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
