---
id: "82856f66-75ee-4a7f-be84-c268482a7190"
type: "notatka-pl"
---
# Optymalizacja zużycia tokenów Claude za pomocą niestandardowych umiejętności

Treść przedstawia strategiczne podejście do interakcji z Claude, które drastycznie redukuje zużycie tokenów bez utraty jakości wyników. Autor demonstruje zmniejszenie zużycia tokenów z 47 milionów do 19 milionów dla tego samego projektu i obciążenia pracy poprzez wdrożenie pięciu specyficznych „umiejętności” (niestandardowych instrukcji/plików Markdown). Główna teza zakłada, że marnotrawstwo tokenów występuje głównie poprzez redundantne ładowanie kontekstu i nieprawidłowe duże wdrożenia, co można złagodzić poprzez dodanie „tarcia” i strukturyzowanych punktów kontrolnych do przepływu pracy AI.

## Umiejętność 1: Auto Compactor
Jest to umiejętność o największym wpływie, zapewniająca największe oszczędności kosztów poprzez rozwiązanie problemu „nadmiernego kontekstu”, który występuje podczas długich sesji, gdzie te same pliki są wielokrotnie odczytywane w wielu kolejnych krokach.

*   **Problem:** W standardowej sesji Claude ponownie odczytuje te same pliki (np. logowanie, sesja, j.et) za każdym razem, gdy wysyłane jest kolejne zapytanie, co prowadzi do wykładniczego wzrostu zużycia tokenów.
*   **Rozwiązanie:** Plik Markdown w folderze umiejętności, który jest uruchamiany na podstawie określonych warunków:
    * Ten sam plik jest odczytywany więcej niż dwa razy.
    * Sesja przekracza 30 kroków.
    * Użytkownik stwierdza „działasz wolno.”
*   **Mechanizm:** Po uruchomieniu Claude podsumowuje ostatnie 10 kroków w pięciu punktach, wykonuje polecenie `/compact` i kontynuuje.
*   **Konkretny wpływ:** Zmniejszenie zużycia tokenów dla konkretnego zadania z 3,2 miliona tokenów do 780 000 tokenów (około 4 razy taniej).

**Kluczowe cytaty**
* „Ten sam plik odczytany więcej niż dwa razy, sesja powyżej 30 kroków lub stwierdzasz, że działam wolno.”
* „Bez umiejętności Claude zużył 3,2 miliona tokenów, z nią 780 000.”

## Umiejętność 2: Review Before Run
Ta umiejętność działa jako bramka jakości, zapobiegając generowaniu przez AI ogromnych ilości błędnego kodu, który użytkownik musi później debugować na własny koszt.

*   **Problem:** Claude może wykonać „opiniotwórczą refaktoryzację” dotykającą wiele plików (np. siedem plików), która zawiera błędy, zmuszając użytkownika do zapłaty zarówno za błędny kod, jak i późniejsze poprawki.
*   **Rozwiązanie:** Obowiązkowa bramka przed każdą edycją wielu plików. Claude musi wygenerować trzy konkretne punkty:
    1. Co się zmieni?
    2. Co może się zepsuć?
    3. Orientacyjnie, ile tokenów zostanie zużytych?
*   **Matematyka:** Błędna implementacja może kosztować 8 000 tokenów wyjściowych, podczas gdy 50-wyrazowy plan kosztuje tylko 80 tokenów.

**Kluczowe cytaty**
* „30 sekund tarcia oszczędza ci tysiące zmarnowanych tokenów.”
* „Błędna implementacja kosztuje 8 000 tokenów wyjściowych. 50-wyrazowy plan kosztuje 80.”

## Umiejętność 3: Spec First
Ta umiejętność zmienia kolejność rozwoju, aby zapewnić walidację logiki przed napisaniem jakiegokolwiek kodu, unikając „pętli przepisywania”.

*   **Problem:** „Klasyczne przejście” obejmuje pisanie kodu → pisanie testów zgodnych z kodem → odkrywanie przypadku brzegowego → przepisywanie wszystkiego. Skutkuje to płaceniem za dwa pełne przejścia.
*   **Rozwiązanie:** Obowiązkowa pięciolinijkowa specyfikacja obejmująca:
    * Wejścia
    * Wyjścia
    * Przypadki brzegowe
    * Tryby awarii
    * Kryteria akceptacji
*   **Przepływ pracy:** Specyfikacja → Zatwierdzenie przez użytkownika → Testy (na podstawie specyfikacji) → Kod (przechodzi testy).
*   **Konkretny wpływ:** Zmniejszenie kosztu z 6 500 tokenów w dwóch przepisaniach do 3 300 tokenów (2 razy taniej).

**Kluczowe cytaty**
* „Claude pisze kod do rejestracji. Następnie pisze testy zgodne z kodem. Następnie odkrywasz przypadek brzegowy, który pominął Claude. Wszystko jest przepisywane.”
* „Jedno przejście testów, którym naprawdę ufasz.”

## Umiejętność 4: Test Writer
Ta umiejętność wykorzystuje fakt, że AI ma już odpowiedni plik w swoim bezpośrednim kontekście, aby zautomatyzować pisanie testów.

*   **Problem:** Użytkownicy często pomijają testy („Dodam testy później”) lub proszą o testy po wyczyszczeniu kontekstu, co jest droższe.
*   **Rozwiązanie:** Hak po użyciu narzędzia. Za każdym razem, gdy Claude zapisuje plik źródłowy, umiejętność automatycznie:
    * Wykrywa framework (np. Jest vs. PyTest).
    * Pisze testy zgodne z istniejącym stylem.
    * Uruchamia testy i zatrzymuje się, jeśli zawiodą.
*   **Konkretny wpływ:** 3 razy tańsze niż proszenie o testy po fakcie.

**Kluczowe cytaty**
* „Pisanie testów od zera jest nudne. Ale Claude właśnie miał plik w kontekście dla edycji, którą napisał.”
* „Trzy razy tańsze niż proszenie: napisz mi testy dla X po fakcie.”

## Umiejętność 5: Plan or Stop
Służy jako „wyłącznik awaryjny” dla wysokiego ryzyka, dużych zmian architektonicznych.

*   **Problem:** Szerokie promptowanie, np. „zrefaktoruj system autoryzacji”, może prowadzić do „splątania”, gdzie półimplementowane pomysły niszczą repozytorium, kosztując więcej w naprawie niż w rozpoczęciu od nowa.
*   **Rozwiązanie:** Umiejętność skanuje pod kątem „sygnałów dużych zadań” (słowa kluczowe: przepisz, zmigruj, zrefaktoruj wszystko). Jeśli zostaną znalezione, Claude musi się zatrzymać i przedstawić 4-punktowy plan:
    1. Pliki objęte zmianami
    2. Kolejność działań
    3. Plan wycofania
    4. Szacowany koszt
*   **Konkretny wpływ:** Zapobiega „katastrofom”, które mogą kosztować 30 000 tokenów, zastępując je planem za 400 tokenów.

**Kluczowe cytaty**
* „Wyłącznik awaryjny dla dużych zadań.”
* „Zła implementacja dużego zadania łatwo kosztuje 30 000 tokenów. Plan kosztuje 400.”

## Kluczowe wnioski, spostrzeżenia i kontekst

**Główna teza:** Efektywność tokenów w LLM do kodowania nie polega na promptowaniu „lepiej” w jednym kroku, ale na wdrażaniu **strukturalnych ograniczeń** i **bramek walidacyjnych**, które zapobiegają redundantnemu przetwarzaniu i katastrofalnym błędom.

**Ranking wpływu umiejętności:**
1.  **Auto Compactor:** Najwyższy zwrot z inwestycji; rozwiązuje systemowy problem rozdętego kontekstu.
2.  **Review Before Run:** Zapobiega kosztownym, dużym halucynacjom/błędom.
3.  **Spec First:** O połowę zmniejsza koszt nietrywialnych funkcji, eliminując pętle przepisywania.
4.  **Test Writer:** Zwiększa pokrycie testów i zmniejsza koszt, wykorzystując „gorący” kontekst.
5.  **Plan or Stop:** Łagodzenie ryzyka dla zmian w całym repozytorium.

**Praktyczne wskazówki:**
*   Wdróż folder `skills` w swoim repozytorium zawierający pliki Markdown definiujące te zachowania.
*   Wprowadź celowe „tarcie” (kroki zatwierdzenia), aby uniknąć wysokiego kosztu poprawiania dużych błędów AI.
*   Przejdź z przepływu pracy „Kod → Test” na „Specyfikacja → Test → Kod”.