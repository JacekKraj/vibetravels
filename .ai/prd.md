Dokument wymagań produktu (PRD) - VibeTravels

**1. Przegląd produktu**

VibeTravels to aplikacja webowa wykorzystująca sztuczną inteligencję do konwersji prostych notatek o planowanych wycieczkach w szczegółowe plany podróży. Aplikacja skierowana jest do grup przyjaciół (do 8 osób pełnoletnich) i umożliwia im efektywne planowanie angażujących wycieczek na podstawie ich preferencji, budżetu oraz dostępnego czasu.

MVP aplikacji zawiera system zarządzania notatkami, prosty system kont użytkowników, stronę profilu z preferencjami turystycznymi oraz integrację z AI, która konwertuje notatki w konkretne, praktyczne plany wycieczek.

Aplikacja umożliwia planowanie wycieczek bez ograniczeń geograficznych, z uwzględnieniem specyficznych preferencji grupy, zapewniając optymalne wykorzystanie dostępnego czasu i budżetu. Plany generowane są automatycznie z możliwością iteracyjnego udoskonalania poprzez system feedbacku.

VibeTravels jest projektowany jako aplikacja webowa z responsywnym designem, skupiająca się na łatwości obsługi i praktyczności dostarczanych informacji.

**2. Problem użytkownika**

Planowanie angażujących i interesujących wycieczek jest trudne i czasochłonne. Użytkownicy napotykają na szereg wyzwań:

*   Trudność w znalezieniu atrakcji dopasowanych do preferencji całej grupy
*   Problem z ułożeniem atrakcji w logicznej kolejności uwzględniającej czas, odległości i godziny otwarcia
*   Konieczność przeszukiwania wielu źródeł informacji o cenach biletów, godzinach otwarcia i potencjalnych zniżkach
*   Trudność w oszacowaniu całkowitych kosztów wycieczki z podziałem na poszczególne elementy
*   Brak pewności co do jakości i atrakcyjności wybranych miejsc

Istniejące rozwiązania często wymagają ręcznego komponowania planu z wielu źródeł lub korzystania z gotowych propozycji, które nie uwzględniają specyficznych preferencji i ograniczeń grupy.

VibeTravels rozwiązuje te problemy poprzez automatyzację procesu planowania przy wykorzystaniu AI, które uwzględnia indywidualne preferencje uczestników, budżet, czas oraz inne czynniki wpływające na jakość wycieczki.

**3. Wymagania funkcjonalne**

    **3.1 System kont użytkowników**
        *   Rejestracja nowego konta przy użyciu adresu email i hasła
        *   Logowanie do istniejącego konta
        *   Profil użytkownika zawierający:
            *   Wykluczenia dotyczące transportu
            *    Preferencje przemieszczania się
            *    Typ preferowanych wakacji (relaksacyjny/aktywny)
            *    Inne informacje związane z preferencjami turystycznymi

    **3.2 System notatek o wycieczkach**
        *   Formularz wprowadzania danych o planowanych wycieczkach zawierający:
            *   Punkt startowy i docelowy
            *   Preferowany sposób dotarcia do punktu docelowego i powrotu do punktu startowego
            *   Planowane miejscowości
            *   Termin i czas trwania
            *   Intensywność wycieczki
            *   Wielkość grupy (do 8 osób)
            *   Budżet per osoba
            *   Dodatkowe notatki od użytkownika

        *   Zapisywanie, przeglądanie, edycja i usuwanie wprowadzonych notatek

    **3.3 Generowanie planów przez AI**
        *   Automatyczna konwersja notatek na szczegółowe plany wycieczek
        *   Dostosowanie do preferencji grupy i budżetu
        *   Lista atrakcji w logicznej kolejności
        *   Uwzględnianie praktycznych informacji (ceny biletów, zniżki, godziny otwarcia, potencjalne kolejki)
        *   Sugerowanie alternatywnych atrakcji
        *   Ogólne sugestie dotyczące zakwaterowania i wyżywienia
        *   Szacowanie kosztów dla poszczególnych elementów planu oraz całkowita suma per osoba

    **3.4 System feedbacku i iteracji**
        *   Przesyłanie uwag do wygenerowanego planu w formie prostej notatki tekstowej
        *   Iteracyjne poprawianie planu przez AI z możliwością wielokrotnych iteracji
        *   Akceptacja finalnej wersji planu, która zostaje zapisana na profilu użytkownika

    **3.5 Interfejs użytkownika**
        *   Formularz preferencji w postaci kilku prostych kroków z wizualną reprezentacją wyborów
        *   Wizualna oś czasu/mapa dla prezentacji planów wycieczek
        *   Responsywny design z naciskiem na czytelność planów na urządzeniach mobilnych
        *   Jasne rozgraniczenie między informacjami obowiązkowymi a opcjonalnymi w formularzu

**4. Granice produktu**

    **4.1 Co wchodzi w zakres MVP:**
        *   System kont użytkowników (rejestracja, logowanie, profil)
        *   Zapisywanie, odczytywanie, przeglądanie i usuwanie notatek o przyszłych wycieczkach
        *   Profil użytkownika z preferencjami turystycznymi
        *   Integracja z AI (OpenAI) do konwersji notatek w szczegółowe plany
        *   System feedbacku do iteracyjnego poprawiania wygenerowanych planów
        *   Informacje praktyczne o atrakcjach (ceny, godziny otwarcia)
        *   Szacowanie kosztów wycieczki (per element + całość)
        *   Ogólne sugestie dotyczące zakwaterowania i wyżywienia
        *   Standardowe zabezpieczenia danych użytkowników
        *   Responsywny design aplikacji webowej

    **4.2 Co NIE wchodzi w zakres MVP:**
        *   Współdzielenie planów wycieczkowych między kontami
        *   Bogata obsługa i analiza multimediów (np. zdjęć miejsc do odwiedzenia)
        *   Zaawansowane planowanie czasu i logistyki
        *   Integracja z zewnętrznymi źródłami danych
        *   Bezpośrednia edycja wygenerowanych planów (tylko poprzez feedback)
        *   Oznaczanie planów jako zrealizowane
        *   Integracja z systemami rezerwacji biletów, hoteli itp.
        *   Funkcje społecznościowe (komentarze, polubienia)
        *   Zaawansowane funkcje wizualizacji tras i map

**5. Historyjki użytkowników**

    **Rejestracja i Logowanie**

    *   **US-001: Rejestracja użytkownika**
        *   *Opis:* Jako nowy użytkownik, chcę utworzyć konto w aplikacji, aby móc korzystać z jej funkcjonalności.
        *   *Kryteria akceptacji:*
            *   Formularz rejestracji wymaga podania adresu email i hasła
            *   System weryfikuje unikalność adresu email
            *   System wymaga hasła o odpowiedniej sile (min. 8 znaków)

    *   **US-002: Logowanie użytkownika**
        *   *Opis:* Jako zarejestrowany użytkownik, chcę zalogować się do aplikacji, aby uzyskać dostęp do moich zapisanych notatek i planów.
        *   *Kryteria akceptacji:*
            *   Formularz logowania wymaga podania adresu email i hasła
            *   System weryfikuje poprawność danych logowania
            *   System informuje o nieprawidłowych danych logowania
            *   Po poprawnym zalogowaniu użytkownik jest przekierowany do strony głównej
            *   Sesja użytkownika jest utrzymywana zawsze, do momentu manualnego wylogowania przez uzytkownika

    *   **US-004: Wylogowanie**
        *   *Opis:* Jako zalogowany użytkownik, chcę wylogować się z aplikacji, aby zabezpieczyć swoje konto.
        *   *Kryteria akceptacji:*
            *   Na każdej stronie aplikacji dostępna jest opcja wylogowania
            *   Po wylogowaniu sesja użytkownika jest zakończona
            *   Po wylogowaniu użytkownik jest przekierowany na stronę logowania

    **Profil użytkownika**

    *   **US-005: Uzupełnienie profilu użytkownika**
        *   *Opis:* Jako nowy użytkownik, chcę uzupełnić mój profil o preferencje turystyczne, aby system mógł generować lepiej dopasowane plany.
        *   *Kryteria akceptacji:*
            *   Formularz preferencji podzielony jest na proste kroki z wizualną reprezentacją wyborów
            *   Użytkownik może określić wykluczenia dotyczące transportu
            *   Użytkownik może określić preferencje przemieszczania się
            *   Użytkownik może określić typ preferowanych wakacji (relaksacyjny/aktywny)
            *   System zapisuje preferencje i potwierdza ich zapisanie
            *   Formularz wskazuje, które informacje są obowiązkowe, a które opcjonalne

    *   **US-006: Aktualizacja preferencji turystycznych**
        *   *Opis:* Jako użytkownik, chcę zaktualizować moje preferencje turystyczne, aby dostosować je do zmieniających się potrzeb.
        *   *Kryteria akceptacji:*
            *   Użytkownik ma dostęp do formularza edycji preferencji z poziomu profilu
            *   Formularz jest wypełniony aktualnymi preferencjami użytkownika
            *   Użytkownik może zmienić dowolną preferencję
            *   System zapisuje zaktualizowane preferencje i potwierdza ich zapisanie
            *   Zmiana preferencji nie wpływa na już wygenerowane plany

    *   **US-007: Przeglądanie profilu**
        *   *Opis:* Jako użytkownik, chcę przeglądać swój profil, aby sprawdzić moje aktualne preferencje i dane.
        *   *Kryteria akceptacji:*
            *   Użytkownik ma dostęp do strony profilu z poziomu menu głównego
            *   Strona profilu wyświetla wszystkie preferencje turystyczne użytkownika
            *   Strona profilu zawiera link do edycji preferencji
            *   Strona profilu wyświetla podstawowe dane konta (adres email)

    **Zarządzanie notatkami**

    *   **US-008: Tworzenie nowej notatki o wycieczce**
        *   *Opis:* Jako użytkownik, chcę utworzyć nową notatkę o planowanej wycieczce, aby później wygenerować szczegółowy plan.
        *   *Kryteria akceptacji:*
            *   Formularz notatki zawiera pola: punkt startowy, miejsce docelowe, termin, czas trwania, intensywność, wielkość grupy, budżet per osoba
            *   Formularz pozwala na dodanie opcjonalnych dodatkowych notatek tekstowych
            *   System jasno rozgranicza pola obowiązkowe i opcjonalne
            *   System zapisuje notatkę i potwierdza jej zapisanie
            *   Po zapisaniu notatki użytkownik jest przekierowany do listy notatek

    *   **US-009: Przeglądanie listy notatek**
        *   *Opis:* Jako użytkownik, chcę przeglądać listę moich notatek o wycieczkach, aby zarządzać moimi planami.
        *   *Kryteria akceptacji:*
            *   Lista notatek jest dostępna z poziomu menu głównego
            *   Lista wyświetla podstawowe informacje o notatkach: miejsce docelowe, termin, status (z planem/bez planu)
            *   Lista umożliwia sortowanie notatek według daty utworzenia i terminu wycieczki
            *   Lista zawiera przyciski do akcji: szczegóły, edycja, usunięcie, generowanie planu

    *   **US-010: Przeglądanie szczegółów notatki**
        *   *Opis:* Jako użytkownik, chcę przeglądać szczegóły konkretnej notatki, aby przypomnieć sobie jej zawartość.
        *   *Kryteria akceptacji:*
            *   Strona szczegółów notatki wyświetla wszystkie informacje zawarte w notatce
            *   Strona zawiera przyciski do edycji, usunięcia i generowania planu
            *   Jeśli dla notatki istnieje wygenerowany plan, strona zawiera link do tego planu

    *   **US-011: Edycja notatki**
        *   *Opis:* Jako użytkownik, chcę edytować istniejącą notatkę, aby zaktualizować informacje o planowanej wycieczce.
        *   *Kryteria akceptacji:*
            *   Formularz edycji jest wypełniony aktualnymi danymi notatki
            *   Użytkownik może zmienić dowolne pole notatki
            *   System zapisuje zaktualizowaną notatkę i potwierdza jej zapisanie
            *   Jeśli dla notatki istnieje wygenerowany plan, system informuje użytkownika, że edycja notatki może wymagać ponownego wygenerowania planu

    *   **US-012: Usuwanie notatki**
        *   *Opis:* Jako użytkownik, chcę usunąć niepotrzebną notatkę, aby zachować porządek w moich planach.
        *   *Kryteria akceptacji:*
            *   System wymaga potwierdzenia przed usunięciem notatki
            *   Po usunięciu notatki użytkownik jest przekierowany do listy notatek
            *   System informuje o pomyślnym usunięciu notatki
            *   Jeśli dla notatki istnieje wygenerowany plan, system usuwa również ten plan

    **Generowanie planów**

    *   **US-013: Generowanie planu wycieczki**
        *   *Opis:* Jako użytkownik, chcę wygenerować szczegółowy plan wycieczki na podstawie mojej notatki, aby lepiej zorganizować podróż.
        *   *Kryteria akceptacji:*
            *   Generowanie planu jest dostępne z poziomu szczegółów notatki lub listy notatek
            *   System informuje o rozpoczęciu procesu generowania
            *   Generowanie uwzględnia preferencje użytkownika zapisane w profilu
            *   Wygenerowany plan zawiera listę atrakcji w logicznej kolejności
            *   Plan zawiera informacje praktyczne (ceny biletów, godziny otwarcia, potencjalne kolejki)
            *   Plan zawiera ogólne sugestie dotyczące zakwaterowania i wyżywienia
            *   Plan zawiera szacunkowe koszty dla poszczególnych elementów i całkowitą sumę per osoba

    *   **US-014: Przeglądanie wygenerowanego planu**
        *   *Opis:* Jako użytkownik, chcę przeglądać wygenerowany plan wycieczki, aby zapoznać się z jego szczegółami.
        *   *Kryteria akceptacji:*
            *   Plan jest prezentowany w formie wizualnej osi czasu/mapy
            *   Plan wyświetla wszystkie atrakcje w logicznej kolejności
            *   Plan zawiera wszystkie informacje praktyczne
            *   Plan zawiera szacunkowe koszty
            *   Strona planu umożliwia szybkie kopiowanie elementów (adresy, godziny)
            *   Strona planu zawiera opcję wydruku (widok print-friendly)
            *   Strona planu zawiera przyciski do przesłania feedbacku i akceptacji planu

    *   **US-015: Przesyłanie feedbacku do planu**
        *   *Opis:* Jako użytkownik, chcę przesłać feedback do wygenerowanego planu, aby dostosować go lepiej do moich potrzeb.
        *   *Kryteria akceptacji:*
            *   Formularz feedbacku jest dostępny z poziomu strony planu
            *   Formularz umożliwia wprowadzenie prostej notatki tekstowej
            *   System informuje o przyjęciu feedbacku i rozpoczęciu regeneracji planu
            *   Historia feedbacków jest zapisywana i widoczna dla użytkownika

    *   **US-016: Regeneracja planu na podstawie feedbacku**
        *   *Opis:* Jako użytkownik, chcę, aby system zregenerował plan na podstawie mojego feedbacku, dostosowując go lepiej do moich potrzeb.
        *   *Kryteria akceptacji:*
            *   System regeneruje plan uwzględniając feedback użytkownika
            *   System informuje o zakończeniu regeneracji
            *   Zregenerowany plan zachowuje strukturę i elementy pierwotnego planu, z wprowadzonymi zmianami
            *   Użytkownik może porównać pierwotną i zregenerowaną wersję planu
            *   Możliwe są wielokrotne iteracje feedbacku i regeneracji

    *   **US-017: Akceptacja finalnej wersji planu**
        *   *Opis:* Jako użytkownik, chcę zaakceptować finalną wersję planu, aby zapisać go na swoim profilu.
        *   *Kryteria akceptacji:*
            *   Opcja akceptacji planu jest dostępna z poziomu strony planu
            *   Po akceptacji plan jest zapisywany na profilu użytkownika
            *   System potwierdza zapisanie planu
            *   Zaakceptowany plan jest oznaczony jako finalna wersja

    **Zarządzanie planami**

    *   **US-018: Przeglądanie zapisanych planów**
        *   *Opis:* Jako użytkownik, chcę przeglądać listę moich zapisanych planów wycieczek, aby zarządzać moimi podróżami.
        *   *Kryteria akceptacji:*
            *   Lista planów jest dostępna z poziomu menu głównego
            *   Lista wyświetla podstawowe informacje o planach: miejsce docelowe, termin, status
            *   Lista umożliwia sortowanie planów według terminu wycieczki
            *   Lista zawiera przyciski do akcji: szczegóły, usunięcie, drukowanie

    *   **US-019: Usuwanie zapisanych planów**
        *   *Opis:* Jako użytkownik, chcę usunąć niepotrzebne plany, aby zachować porządek w moim profilu.
        *   *Kryteria akceptacji:*
            *   System wymaga potwierdzenia przed usunięciem planu
            *   Po usunięciu planu użytkownik jest przekierowany do listy planów
            *   System informuje o pomyślnym usunięciu planu
            *   Usunięcie planu nie wpływa na powiązaną notatkę

**6. Metryki sukcesu**

    **6.1 Metryki angażowania użytkowników**
        *   90% użytkowników posiada wypełnione preferencje turystyczne w swoim profilu
        *   75% użytkowników generuje 3 lub więcej planów wycieczek rocznie
        *   70% użytkowników korzysta z funkcji feedbacku przynajmniej raz

    **6.2 Metryki jakości generowanych planów**
        *   80% użytkowników prosi o maksymalnie jedną edycję planu przed jego akceptacją
        *   90% użytkowników akceptuje wygenerowane plany po maksymalnie dwóch iteracjach feedbacku

    **6.3 Metryki wydajności systemu**
        *   Średni czas generowania planu poniżej 60 sekund
        *   Średni czas regeneracji planu na podstawie feedbacku poniżej 30 sekund
        *   Dostępność systemu na poziomie 99%
        *   Czas ładowania stron poniżej 2 sekund

    **6.5 Metryki techniczne**
        *   Liczba błędów zgłaszanych przez użytkowników poniżej 5 tygodniowo
        *   95% wygenerowanych planów zawiera wszystkie wymagane elementy
        *   98% poprawnych szacunków kosztów (w granicach 10% rzeczywistych cen)