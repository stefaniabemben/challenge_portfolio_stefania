# TASK 1
## Subtask 1
#### 8 punktów
## Subtask 3
#### Cześć! Nazywam się Stefania. Pół roku temu podjęłam ważną decyzję o całkowitej zmianie ścieżki zawodowej- lada moment ukończę kurs "Tester Oprogramowania". :mag: 
#### Biorę udział w wyzwaniu ponieważ wierzę, że pozwoli mi ono pogłębić wiedzę z zakesu testowania manualnego, doda mi "praktycznych skrzydeł" oraz przygotuje mnie do podjęcia pierwszej pracy w tej branży. 🎯
#### Stefania
## Subtask 4
#### Aplikacja https://scouts-test.futbolkolektyw.pl/pl

### Na czym polega ta aplikacja? Do czego służy?

#### Aplikacja umożliwia zalogowanie się, dodawanie graczy do bazy, przeglądanie dodanych już graczy, przelądanie ich wyników, pozyskiwanie kontaktu do nich oraz innych informacji na temat ich gry. Dodatkowo w alikacji można zobaczyć raporty dotyczące konkretnych graczy oraz rozegrane przez nich mecze oraz zasymulować rozgrywkę meczu. 


### Jakie funkcjonalności znajdują się w aplikacji? Do czego służą. Czy są intuicyjne, czy może byś coś zmienił_a? (Nie bój się wyrażać opinię!)
#### Funkcjonalności znajdujące się w aplikacji: zalogowanie się, wylogowanie się, dodanie gracza, przeglądanie bazy danych z graczmi dodanymi, możliwość odszukania konkretnego gracza za pomoca pola "search", edycja dodanych już graczy, możliwośc generowania raportów, możliwość symulacji rozgrywki, możliwość edycji oraz dodania meczu oraz możliwość podglądu ostatniej aktywności w aplikacji. 

#### Funkcjonalności są dość intuicyjne, np logowanie się jest łatwe i zrozumiałe. Możliwość dodania nowego gracza za pomocą buttonu "Dodaj gracza" na środku jest zrozumiała i łatwa, przeglądanie dodanych już graczy jest intuicyjne. Przeglądanie meczy oraz raportów danego gracza też jest dość zrozumiałe. Button "Wyloguj" jest dobrze widoczny na końcu menu. 


### Oceń interfejs aplikacji (wygląd) – czy Ci się podoba, czy nie?
#### Interfejs aplikacji nie podoba mi się, jest bardzo surowy, wygląda jak suchy formularz, nie zachęca do korzystania. 

### Czy aplikacja jest intuicyjna? (Intuicyjna, czyli np. nie masz problemu ze zrozumieniem, co należy kliknąć, żeby wejść do formularza dodawania nowego zawodnika piłki nożnej do systemu).
#### W aplikacji intuicyjne są działania związane z głównymi funkcjonalnościami, np. logowanie, dodawanie gracza. Natomiast po przejściu do strony umożliwiającej dodanie gracza aplikacja pozostawia wiele do życznia. Pola do uzupełnienia nie są w należyty sposób wyjaśnione. Na przykład pole "profil na facebooku" nie wyjaśnia w żaden sposób czy powinna to być nazwa profilu czy link, pole "Łączy nas piłka" oraz pole "90 minut" również nie są zrozumiałe, ciężko wywnioskować jakie informacje powinny się tam znaleźć. Dodatkowo w zakłądce "Mecze" nieintuicyjna jest według mnie symulacja meczu (button "Rozpocznij mecz"). Nie zostało tam wyjaśnione działanie danego meczu, możliwe ruchy - dopiero w procesie eksploracji można zorientować się o co chodzi. Dodawanie nowych raportów nie jest możliwe z poziomu zakładki "Raporty" mimo, że jest tam poświęcony temu button - kieruje on do zakłądki "Mecze" i dopiero po dodaniu nowego meczu możemy dołączyć do niego raport - więc dodawanie nowych raportów nie jest intuicyjne - również można dotrzeć do tego dopiero po eksploracji. Nieintuicyjny jest również według mnie fakt, że nie dodano buttonu "Dodaj gracza" do menu po lewej stronie. 

### Czy zauważasz jakieś błędy? Albo coś wydaje Ci się błędem? Zapisz swoje przemyślenia w pliku. Tutaj masz na to miejsce, czas i przestrzeń! ;)
#### Błędy jakie znalazłam (testowanie eksploracyjne): 
#### 1. Podczas dodawania gracza, po wypełnieniu formularza, pojawia się informacja "Nie udało się dodać gracza" lecz błędnie wypełnione pola nie są w żaden sposób wskazane/podpowiedziane.
#### 2. Podczas dodawania gracza, w formularzu można podać ujemne wartości w oknach "Waga" oraz "Wzrost", system przepuszcza to jako poprawną wartość.
#### 3. Podczas dodawania gracza, w formularzu, imieniem oraz nazwiskiem mogą być cyfry.
#### 4. Podczas dodawania gracza, w formularzu, numerem telefonu mogą być litery. 
#### 5. Podczas dodawania gracza, w formularzu, w oknie "Link do Youtube" system pozwala na wpisanie liter, cyf, kombinacji niebędących hiperłączem.
#### 6. Podczas dodawania gracza, w formularzu, system pozwala na dodanie przyszłej daty w oknie "Data urodzenia".
#### 7. Po zmianie języka na język angielski w aplikacji:
   #### - w zakładce "Add player"  niektóre okna nadal wyjaśnione są w języku polskim - okno "Łączy nas piłka" oraz okno "90 minut".
  #### - w oknie "District" do wyboru są dziwne wyniki - miasta, wymyślone określenia itd.
   #### - w zakładce "Matches" po prawej stronie, przy każdym meczu, wyświetlaja się opcje "Edit", "Add report" i "Start report" w wersji polskiej zamiast start raport było "Rozpocznij mecz", więc chodzi tu o mecz czy o raport?
#### 8. W zakładce "Raporty", po wejściu w konkretnego gracza, po lewej stronie u góry pojawia się button "Dodaj raport" - kieruje on do istniejących już meczy, raport można dodać tylko do dodanego już meczu więc button "Dodaj raport" jest niepotrzebny i wpowadzający w błąd.
#### 9. Według mnie błędem jest również to, że każdy może edytować dane wszystkich zawodników, dane meczowe, raporty. Uważam, że możliwość te powinien mieć tylko autor konkretnego wpisu.
#### 10. Podczas edycji meczu część okien wyjaśniona jest w języku polskim, a część w języku angielskim. Dodatkowo data rozegranego meczu może być datą przyszłą, a czas meczu może być ujemny.
#### 11. W raporcie meczowym, w oknie "Link do meczu" można wprowadzić każdy znak, łącznie z emotikoną.
#### 12. Podsumowując - w każdym formularzu w aplikacji można wprowadzać wartości ujemne i daty przyszłe, a okna w których powinna być możliwość wpisania jedynie cyfr dopuszczają też litery oraz na odwrót.

### Komunikaty jakie zostały wyświetlone przez DevTools:
#### 1. A label isn't associated with a form field.
#### 2. An element doesn't have an autocomplete attribute.
#### 3. A form field element has neither an id nor a name attribute. This might prevent the browser from correctly autofilling the form.
#### 4. Params `start` and `limit` are deprecated. Use `_start` and `_limit`


## Subtask 5
#### https://bembenstefania.atlassian.net/jira/software/c/projects/CPP/boards/4?atlOrigin=eyJpIjoiMjkyYmY4YjY5MjA4NDZmYWI2MGM5NDdmNDM5ZmQ1MzMiLCJwIjoiaiJ9





# TASK 2
## Subtask 1
### https://docs.google.com/document/d/1k4ZAYKrZsnLurpbyn12vJUJOCFfBNYjkaLJFR70wLfQ/edit?usp=sharing
## Subtask 2
### https://docs.google.com/document/d/16-8lo_xljnaKcC2OsRL9N51uJCJtCIfooeD6DRB51NU/edit?usp=sharing
## Subtask 3
### Po co piszemy test case'y? 
#### Test case'y są według mnie drogowskazami dla testera :construction: . Wskazują odpowiedni kierunek drogi (steps) oraz pokazują, co powinniśmy na jej końcu znaleźć - nasz cel (expected result) :round_pushpin:. Są zbiorem niezbędnych informacji, kroków i działań, które powinny doprowadzić nas do oczekiwanego rezultatu. Tester to podróżnik, który musi skorzystać z tych podpowiedzi, aby sprawdzić, czy na końcu drogi na pewno jest to, co powinno. :train:
## Subtask 4
### https://docs.google.com/document/d/1-G_Sdx3GO0e50BIi7RgGPQE_eoST4A8mHG2J7dT0D1Q/edit?usp=sharing


# TASK 3
## Subtask 1 i 2
### https://docs.google.com/document/d/1zzCmCirSAxY8QeyQ3Id2DQuTd6h-6-ObgrV8PIytKus/edit?usp=sharing

## Subtask 3
### https://drive.google.com/file/d/1byt0kxRo-8iUGY6Tqhjue9FEtxJ17Ej5/view?usp=sharing
### https://docs.google.com/document/d/1-Zagu3sfCvylMe-xhQvgzoU1o8F-yXlbESPoP3GtoiY/edit?usp=sharing


# TASK 4
## Subtask 1 i 2 
### https://docs.google.com/document/d/1SkUuETJYvgak5-9bt8rQL3JJt1D1QwCa9u9rrT5wohM/edit?usp=sharing

## Subtask 3 
### Do czego służy ta aplikacja? Jaki jest cel tej aplikacji?
#### Aplikacja służy do zamieszczania przedmiotów przeznaczonych na sprzedaż/wymianę/do oddania za darmo oraz umożliwia zakup wystawionych tam przedmiotów (kontakt z osobą wystawiającą ogłoszenie, finalizaja transakcji). Dodatkwo aplikacja ma również opcję zamieszczania ogłoszeń o pracę oraz utworzenia profilu kandydata, który pozwoli na aplikowanie na wyżej wymienione ogłoszenia. 

### Kto ma być użytkownikiem końcowym aplikacji?
#### Użytkownikiem końcowym aplikacji jest osoba poszukująca danego przedmiotu/pracy lub osoba wystawiająca ogłoszenie. 

### Czy według Ciebie aplikacja jest user friendly?
#### Uważam, że aplikacja OLX.pl jest dość przyjazna dla użytkowników. Jest szybka oraz uważam ją za bezpieczną. Moja opinia może wynikać z faktu, iż na codzień wiele z niej korzystam, jenak uważam, że przeciętny użykownik również nie powinien mieć z nią problemów, przynajmniej na sprzęcie, na jakim ja miałam okazję ją testować. Niestety interfejs aplikacji pozostawia wiele do życzenia, nie jest przejżysty. Uważam, że wyszukiwanie produktów w polu "Search" jest intuicyjne natomiast wszystkie produkty pojawiające się na stronie głównej w zakładkach produktów proponowanych, produków obserowanych i produktów ostatnio oglądanych zlewają się w jedną całość. 

### Jak byś usprawnił aplikację? Co byś w niej poprawił. Czy masz jakiś pomysł na dodatkową funkcjonalność? (Żeby nie było: nie jest to aplikacja przy której pracuję, takie pytania pojawiają się na rozmowach rekrutacyjnych dlatego dobrze jest to przećwiczyć :D )
#### Uważam, że obok miniaturek przedmiotów oraz nazwy ogłoszenia powinna być widoczna ikona zawierająca informację, czy można zakupić dany przedmiot z wysyłką. Woalałabym wiedzieć to zanim kliknę w dany przedmiot i wyświetlę o nim pełne informacje. 
#### Dodatkowo interfejs nie jest zbyt przejżysty. Według mnie upożądkowane powinny zostać zakładki z produktami ostatnio oglądanymi, produktami proponowanymi oraz ulubionymi, tak aby nie zlewały się w jedną całość. 

### Jakie dostrzegasz różnice pomiędzy testowaniem aplikacji internetowej, a natywnej?
#### Główną różnicą jaką widzę jest dostosowanie aplikacji natywnej do sprzętu na jakim ją testuję - dostęp do lokalizacji, plików zapisanych na danym sprzęcie oraz dostosowanie interfejsu i systemu, co sprawia, że testowanie jest sprawniejsze i może przebiegać w rzeczywistym środkowisku. Dodatkowo aplikacja natywna jest szybka, działa sprawniej niż aplikacja internetowa. Przy testowaniu aplikacji natywnej mogę się również skupić na aspektach takich jak żywotność baterii podczas korzystania, otrzymywanie powiadomień od aplikacji. 


## Subtask 4 
#### https://bembenstefania.atlassian.net/jira/software/c/projects/CPP/boards/4?atlOrigin=eyJpIjoiMmU1Y2ZkZjg3YzU1NDJkMmEzNjk2MzUyMDM1ZWRlNjQiLCJwIjoiaiJ9


# TASK 5
## Subtask 1 -Kurs podstaw SQL
## Subtask 2
# <img src=”img width="314" alt="Zrzut ekranu 2023-10-11 090703" src="https://github.com/stefaniabemben/challenge_portfolio_stefania/assets/137799832/4fb260d1-3e95-45cd-b73f-ee1e04d0cd7c"” width=”50%” height=”50%”>
## Subtask 3 - Zadania
### 1. Wyświetl tabelę actors w kolejności alfabetycznej sortując po kolumnie surname.
# <img width="460" alt="Zrzut ekranu 2023-10-11 090435" src="https://github.com/stefaniabemben/challenge_portfolio_stefania/assets/137799832/cc0f9b69-fd82-4550-be33-2f35f7426f74">
### 2. Wyświetl film, który powstał w 2019 roku.
# <img width="309" alt="Zrzut ekranu 2023-10-11 091226" src="https://github.com/stefaniabemben/challenge_portfolio_stefania/assets/137799832/4aaa7752-18a8-4723-95ac-df849e31dcdb">
### 3. Wyświetl wszystkie filmy, które powstały między 1900, a 1999 rokiem.
# <img width="341" alt="Zrzut ekranu 2023-10-11 091813" src="https://github.com/stefaniabemben/challenge_portfolio_stefania/assets/137799832/22c214d8-ff08-4cd0-8708-c365d8aa14fd">
### 4. Wyświetl JEDYNIE tytuł i cenę filmów, które kosztują poniżej 7$
# <img width="323" alt="Zrzut ekranu 2023-10-11 092221" src="https://github.com/stefaniabemben/challenge_portfolio_stefania/assets/137799832/f0deaa5a-cd90-429e-9286-4e21b38f470b">
### 5. Użyj operatora logicznego AND, aby wyświetlić aktorów o actor_id pomiędzy 4-7 (4 i 7 powinny się wyświetlać). NIE UŻYWAJ operatora BETWEEN.
# <img width="317" alt="Zrzut ekranu 2023-10-11 092708" src="https://github.com/stefaniabemben/challenge_portfolio_stefania/assets/137799832/3f7b5ddd-c063-4114-8386-845a72bcffb8">
### 6. Wyświetl klientów o id 2,4,6 wykorzystaj do tego warunek logiczny.

### 7. Wyświetl klientów o id 1,3,5 wykorzystaj do tego operator IN.
# <img width="366" alt="Zrzut ekranu 2023-10-11 093424" src="https://github.com/stefaniabemben/challenge_portfolio_stefania/assets/137799832/c19ea2dd-e25c-4450-a46b-4f6f6c0cf1a4">
### 8. Wyświetl dane wszystkich osób z tabeli ‘actors’, których imię zaczyna się od ciągu “An”.

### 9. Wyświetl dane klienta, który nie ma podanego adresu email.

### 10. Wyświetl wszystkie filmy, których cena wynosi powyżej 9$ oraz ich ID mieści się pomiędzy 2 i 8 movie_id.
# <img width="357" alt="Zrzut ekranu 2023-10-11 113322" src="https://github.com/stefaniabemben/challenge_portfolio_stefania/assets/137799832/3dd45ca4-c843-48cf-a74d-78b7dc7c9c9a">
