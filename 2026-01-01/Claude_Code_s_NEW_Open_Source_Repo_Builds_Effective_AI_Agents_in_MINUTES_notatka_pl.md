---
id: "ea182c2e-5237-4e5a-bb7d-8582340b4b3f"
---

---

# Analiza: Umiejętność "Uruchom swojego agenta" dla Claude Code

**STRESZCZENIE**
Treść przedstawia umiejętność "Uruchom swojego agenta", darmowe, otwartoźródłowe narzędzie dla Claude Code, które umożliwia użytkownikom przejście od koncepcji do działającego, hostowanego w chmurze agenta AI w ciągu kilku minut. Kluczową zmianą jest przejście od "podawania poleceń" do "pętli", gdzie użytkownik definiuje cele i kryteria sukcesu, zamiast szczegółowych instrukcji krok po kroku. Umiejętność automatyzuje wdrażanie Zarządzanych Agentów Claude (CMA), które działają autonomicznie na serwerach Anthropic, wykorzystując samodoskonalącą się pętlę sprzężenia zwrotnego i opcjonalne magazyny pamięci. Chociaż demonstracja pokazuje moc tej automatyzacji, ujawnia również kluczowe wyzwania związane z uprawnieniami środowiska (np. dostęp do Reddita) oraz potencjalnie wysokimi kosztami tokenów podczas pętli błędów.

---

### 1. Zmiana paradygmatu: od czatowania do pętli
Główna teza mówi, że prawdziwa automatyzacja wymaga agentów - które posiadają narzędzia i autonomię - a nie prostych interfejsów czatu. Autor wprowadza nową warstwę abstrakcji w kodowaniu, gdzie rola człowieka zmienia się z pisania kodu lub poleceń na projektowanie "pętli".

*   **Agent AI vs. Czat:** Czat jest ograniczony do słów; agent jest jak "pracownik" z narzędziami (wyszukiwanie w sieci, zapisywanie plików, wykonywanie kodu, wywołania API) i autonomią w wyborze narzędzia na każdym kroku.
*   **Koncepcja "pętli":** 
    *   **Zorientowana na cel:** Użytkownik podaje *cel*, a nie *zadanie*.
    *   **Cykl:** Agent myśli $\rightarrow$ wybiera narzędzia $\rightarrow$ wykonuje $\rightarrow$ odczytuje wyniki $\rightarrow$ samoocenia.
    *   **Samokorekta:** Jeśli wyniki nie spełniają "kryteriów sukcesu", agent wraca do fazy myślenia i powtarza proces, aż wynik będzie zadowalający.
*   **Rola człowieka:** Człowiek dostarcza trzy kluczowe informacje:
    1.  **Kontekst:** Osobiste preferencje lub istniejące bazy danych.
    2.  **Cel:** Co należy osiągnąć.
    3.  **Sukces:** Jasna definicja idealnego wyniku („rubryka”).

**Kluczowe cytaty**
*   "Jeśli chcesz, aby AI wykonywało dla ciebie powtarzalną pracę bez twojej ingerencji, potrzebujesz agenta, a nie tylko lepszego polecenia."
*   "Już nie podaję poleceń Claude’owi. Moim zadaniem jest pisanie pętli, a Claude w zasadzie podaje polecenia sam sobie."
*   "Możesz to postrzegać jako samodoskonalącą się pętlę sprzężenia zwrotnego, w której jako człowiek nie jesteś już odpowiedzialny za wyniki Claude’a - on jest odpowiedzialny za swoje własne wyniki."

---

### 2. Zarządzani Agenci Claude (CMA) i infrastruktura techniczna
Umiejętność "Uruchom swojego agenta" upraszcza wdrażanie CMA, eliminując potrzebę zarządzania przez użytkownika własnymi serwerami lub infrastrukturą.

*   **Hosting w chmurze:** CMA są hostowane na serwerach Anthropic, co oznacza, że są "zawsze włączone" i mogą być zaplanowane do automatycznego uruchamiania, niezależnie od aktywności komputera użytkownika.
*   **Struktura kosztów:** Nie ma dodatkowych opłat platformowych za korzystanie z CMA; użytkownicy płacą tylko standardowe koszty API.
*   **Magazyn pamięci:** Agenci mogą być podłączeni do magazynu pamięci, co pozwala im zachować informacje między sesjami i poprawiać wydajność w czasie.
*   **Umiejętność "Zakończ":** Dodatkowa umiejętność, która zamyka projekty, tworzy przeglądową stronę budowy i sugeruje 1-2 konkretne ulepszenia dla agenta.

**Kluczowe cytaty**
*   "Anthropic będzie obsługiwać pętlę dla ciebie, będzie ją hostować w chmurze na swoich serwerach."
*   "Stary sposób polegał na tym, że musiałbyś sam zbudować tę pętlę, musiałbyś uruchomić własny serwer, musiałbyś rozwiązywać własne błędy."

---

### 3. Proces wdrażania i demonstracja
Autor demonstruje instalację i wdrożenie agenta "Codzienny przegląd wiadomości AI".

*   **Instalacja:** Umiejętność jest instalowana globalnie w Claude Code poprzez link do repozytorium GitHub.
*   **Proces wywiadu:** Umiejętność nie rozpoczyna budowy od razu; przeprowadza wywiad z użytkownikiem w celu zdefiniowania:
    *   **Wyników:** (np. historia z linkiem, haczyk tematyczny i sekcja "dlaczego to ważne").
    *   **Niszy/odbiorców:** (np. entuzjaści AI i Claude Code).
    *   **Źródeł:** (np. konkretne subreddity, takie jak r/Claude lub r/Anthropic).
    *   **Rubryki wyniku:** Ścisły zestaw zasad (np. dokładnie pięć pozycji, działające linki, brak duplikatów, czysty markdown).
*   **Wdrożenie:** Po zatwierdzeniu planu (użytkownik zmienił model z Opus na Sonnet dla wydajności), umiejętność obsługuje wywołania API, uruchamianie środowiska i harmonogramowanie.
*   **Monitorowanie:** Użytkownicy mogą śledzić postęp za pomocą wygenerowanej przeglądowej tablicy HTML lub przeglądając sesje na platforma.claude.com.

**Kluczowe cytaty**
*   "Umiejętność przeprowadzi z tobą wywiad. Zapyta cię, co ma zrobić i czym jest sukces, ponieważ agent nie będzie wiedział, kiedy skończyć, jeśli nie zrozumie, co oznacza sukces."
*   "Możesz poświęcić 10 minut teraz, aby to dobrze ustawić. I to zaoszczędzi ci godzin pracy później."

---

### 4. Podsumowanie: niepowodzenia i wnioski
Demonstracja kończy się analizą "dobre, złe i brzydkie" pierwszego uruchomienia, podkreślając ryzyka związane z autonomicznymi pętlami.

*   **Niepowodzenie:** Agent przez 28 minut próbował uzyskać bezpośredni dostęp do Reddita z zarządzanego środowiska, co było zablokowane.
*   **"Pułapka tokenów":** Ponieważ agent był w pętli, próbując spełnić kryterium sukcesu "musi zawierać linki z Reddita", wielokrotnie zawodził i ponawiał próby.
*   **Koszt:** Nieudane uruchomienie zużyło około 27 milionów tokenów, kosztując około 12 dolarów.
*   **Rozwiązanie:** Autor sugeruje, aby system weryfikował "teorie" (np. sprawdzał dostępność witryny) *przed* wdrożeniem zarządzanego agenta do chmury.

**Kluczowe cytaty**
*   "Głównym problemem, na który się natknęliśmy, był fakt, że w tym zarządzanym środowisku Claude’a nie można było bezpośrednio uzyskać dostępu do Reddita... to zadanie zajęło 28 minut."
*   "Wydałem sporo tokenów na to. Widzisz, zużyłem około 27 milionów tokenów. To było około 12 dolarów tylko na uruchomienie tego."

---

### Kluczowe wnioski, spostrzeżenia i kontekst

**Główna teza**
Przyszłość produktywności AI odchodzi od ręcznego podawania poleceń na rzecz projektowania autonomicznych, samokorygujących się pętli (CMA), które zarządzają własnym wykonaniem i kontrolą jakości.

**Kluczowe spostrzeżenia**
*   **"Rubryka sukcesu" jest wszystkim:** Zdolność agenta do ukończenia zadania zależy wyłącznie od tego, jak konkretnie użytkownik definiuje "sukces". Niejasne cele prowadzą do nieskończonych pętli lub słabej jakości.
*   **Niebezpieczeństwo autonomicznych pętli:** Chociaż samokorekta jest zaletą, może stać się finansowym obciążeniem, jeśli agent napotka twardą przeszkodę (np. zaporę sieciową lub ograniczenie API), ale jest instruowany, aby próbować, aż odniesie sukces.
*   **Wybór modelu ma znaczenie:** Autor zauważył, że modele o wysokiej zdolności rozumowania, takie jak Opus, mogą być przesadą dla prostych zadań (np. przeglądów wiadomości), sugerując Sonnet dla lepszej efektywności kosztowej i szybkości.

**Praktyczne wskazówki dla użytkowników**
*   **Kontrola przed startem:** Przed wdrożeniem CMA ręcznie zweryfikuj, czy narzędzia i źródła potrzebne agentowi są rzeczywiście dostępne w środowisku chmurowym.
*   **Zacznij od prostych rozwiązań:** Wykorzystaj fazę "wywiadu" umiejętności, aby doprecyzować głos i ograniczenia agenta przed pierwszym uruchomieniem.
*   **Monitoruj koszty:** Uważnie śledź zużycie tokenów podczas pierwszych kilku uruchomień nowej pętli, aby uniknąć "pułapek tokenowych" spowodowanych powtarzającymi się błędami.

---