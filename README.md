# challenge_portfolio_Marek

## SPIS TREŚCI
1. [TASK 1](#TASK1)

2. [TASK 2](#TASK2)

3. [TASK 3](#TASK3)

4. [TASK 4](#TASK4)

5. [TASK_5](#TASK5)

<div id='TASK1'/>

## TASK 1 

### Subtask 1

Wyciągamy karteczki - **7/10**

### Subtask 3

<p align="justify"> 
Cześć, Mam na imię Marek. Dołączyłem do projektu ponieważ chcę się przebranżowić. Zacząłem samodzielnie (no dobra, ze wsparciem znajomych z IT i brata, który jest testerem automatyzjącym i też się przebranżowił) przygotowywać się do tego "projektu". Zagadnienia teoretyczne zgłębiam z internetu, czytam sylabus ISTQB (kto go napisał powienien ponieść karę), książki, tutoriale itd. Szukałem programu, który da mi możliwość nabycia praktycznych umiejętności. I to jest mój cel i oczekiwanie wobec udziału w challenge portfolio.
</p>

### Subtask 4

<p align="justify">
Aplikacja służy do śledzenia, raportowania i ewaluacji występów poszczególnych zawodników w meczach piłkarskich. Dzięki rankingom i szczegółowym raportom dotyczącym poszczególnych zawodników możeliwe jest wyłowienie obiecujących piłkarzy, śledzenie postępów w rozwoju zawodnika
  
 **Funkcje Aplikacji**
  
  * Dodawnia nowego zawodnika
  
  * Edycja danych zadownika
  
  * Dodanie rozgrywanego meczu przez danego zawodnika wraz z szczegółowymi informacjami - czas trwania, wynik, drużyny
 
  * Edycja danych meczu
  
  * Dodanie raportu zawodnika z meczu - szczegółowe dane dotyczące występu gracza - jego skuteczności, podjętych akcji wraz z możliwością szerszego opisowego
  komentowania
  * Edycja raportów
  * "rozpoczecie meczu" - użytkownik, może w czasie rzeczywistym lub po czasie odtworzyć występ danego piłkarza dodając wykonane akcje, ich skuteczność (takie jak np. podaniam strzały, dośrodkowania) - informacje zapisane trafiają atomatycznie do utworzonego raportu
  * aplikacja rozróżnia pozycje gracza - inne jest widok meczu oraz możliwego wyboru działań dla bramkarza a inna dla zawodników grających w polu. Aplikacja rozpoznaje polskie i angielskie nazwy pozycji gracza. 
  * aplikacja ma funkcje logowania do systemu, więc wszystkie funkcjonalności dostępne są tylko dla zarejestrowancyh użytkowników
  * Aplikacja występuje w wersji polsko i angielskojęzycznej z możliwości przełączania języka w menu bocznym
  
 Korzystanie z aplikacji wymaga przyzwyczajenia się, aplikacje nie jest intuicyjna. 
  * Dodanie gracza możliwe jest tylko z pozycji strony głównej. Wchodząc w listę graczy - nie ma możliwości dodania nowego zawodnika
  * Brakuje w menu głównym linków do zakładek - mecze i raporty. Żeby się do nich dostać - trzeba "wejść" przez zawodnika
  * Tworzenie raportu również jest mało przyjazne. Przycisk "dodaj raport" nie działa - prowadzi użytkownika do zakładki "mecze". Dodanie raport jest możliwe jedynie przez ikonkę w zakładce mecze. Raport będzie również pełny tylko wtedy jeśli "odegrany" mecz, co moża zrobić tylko z pozycji zakłądki "mecze"
  * Trzeba pamiętać o "uplodowania" odegranego meczu, inaczej dane wprowadzone zostaną utracone. System nie ostrzega przed utratą danych
  * Nie da się wejść w szczegóły meczu czy raportu kilkając na pole danego meczu/raportu. Jedyna opcja to edytowanie meczu/raportu. Tylko wtedy możemy zobaczyć szczegóły
  * na stronie głównej mamy kafelki z zbiorczą inoformacją na temat liczny zawodników, meczy, raportów, akcji. Ale kafelki nie są interkatywne. Nie prowadzą do zbiorczych danych z danego obszaru. Nie wiadomo do końca po co się tam znajdują. 
  
  **Interfejs**
  
  Aplikacja jest bardzo oszczędna, korzysta z prostego layouty, jest przejrzysta, ale mało atrakcyjna dla użytkownika
  
  **Błędy**
  Podczas testów znalazłem 10 błędów oraz 6 rozwiązań funkcjonalnych, które budzą moje wątpliwości
  
 * Błędy
    * System nie ostrzega przed utratą niezapisanych danych przy zamknieciu utworzonych akcji z meczu
    * Przycisk "dodaj raport" w zakładce "raporty" nie działa. Zamiast dodania rpoartu prowadzi do sekcji "mecze"
    * W edytorze raportu nie działają listy (numeryczna i punktowa)
    * Pola z informacjami o zawodniku (imię, nazwisko, klub itd) nie mają ograniczenia ilości znaków. Przez co lista graczy się "wysypuje" kiedy ktoś wprowadzi bardzo długi ciąg znaków w opisie
    * System przyjmuje zdublowane dane zawodników. Można tworzyć dowolną ilość zawodników o tych samych danych
    * System przyjmuje ujemne wartości liczbowe przy polach "czas gry" i "numer zawdonika" w edycji meczu
    * W formularzu zawdonika pole "wiek" przyjmuje liczby ujemne oraz 0
    * Pola, gdzie uzupełnia się dane zawodnika przyjmują emotikony
    * Pole "imię" w zakladce zawdonika przyjmuje dane liczbowe
 
 * Funkcje
    * Brak opisów do przycisków w oknie dodawnia akcji z meczu
    * Podczas wprowadzenia nieporpawnego maila, system wyświetla nieprecyzyjny komunikat o błędzie. Użytkownik nie ma informacji o tym co zrobił źle
    * Brak podlinkowania do zakładek "mecze" i "raporty" z pozycji strony głównej
    * Brak możliwości wejścia w szczegóły meczu/raportu klikając na pole danego meczu. Trzeba wejść przed edycję, 
    * Pola w opisie zawodnika (imię, nazwisko, klub) przyjmują znaki specjalne (np. $%^&*)
    * Pole Login traktuje spację jako znak
</p>
<div id='TASK2'/>

## TASK 2 

### Subtask 1 - Pisanie przypadków testowych na podstawie User Story
  * [Google Drive](https://docs.google.com/spreadsheets/d/19J1OEtKGKX11-fIfb0Emp66YXIwJoCf-C7Y-bSjyd-A/edit#gid=1114735493)
  
### Subtask 2 - Pisanie przypadków testowych na podstawie “własnych doświadczeń.
  * [Google Drive](https://docs.google.com/document/d/1emiIiiXw98dk6WoVdpegFpvS9Kvikx6InbxuMTbQ3PE/edit)
  
### Subtask 3 - Po co piszemy test case’y?

  Test case'y piszemu żeby:
  * uporządkować pracę
  * dokładnie opisać korki testowania, żeby inne osoby mogły z łatwością otworzyć test case - np. inny tester, lub developer, który będzie naprawia buga
  * ułatwić późniejsze testy regresji 
  * wkurzyć testera
 
 <div id='TASK3'/>

## TASK 3

### Subtask 1 - Formularz zgłoszenia błędu
  * [Google Drive](https://docs.google.com/document/d/1QcI35jge0DBu9aUvN8ak1XFMUO8qiH1WKgZn78YZGEA/edit)
  
### Subtask 2 - Testowanie według planów testów i raportowanie błędów
  * [Google Drive](https://docs.google.com/document/d/1PAA5ezU1bROlcqeaI_CjZ5dsitNvBGRqxS6JM-_9jlw/edit)
  
### Subtask 3 - Raport z wykonanych testów
  * [Google Drive](https://docs.google.com/document/d/1YVdhFhwKZkL85KVMVO6GI515c8HXGxTQF45DGcmfUFU/edit)

<div id='TASK4'/>

## TASK 4

### Subtask_1_&_2 - formularz zgłoszenia błędu aplikacja mobilna & zgłoszone błędy
* [Google Drive](https://docs.google.com/document/d/1UUSilt8CK82MVb0oRAyIfbCWvGBz5OQMIR2Opvbc2Fo/edit)

### Subtask 3 - Do czego służy ta aplikacja?

1. **Do czego służy ta aplikacja? Jaki jest cel tej aplikacji?** 

Aplikacja ma na celu dostarczenie użytkownikowi gotowych praktyk, programów medytacyjnych, relaksacyjnych. Promuje i ułatwia dostęp do praktyk mindfulness. Użytkownik dzięki tej aplikacji może wybrać konkretny obszar na jakim chce się skupić (np. redukcja stresu, budowanie uważności, dobre relacje) i aplikacja zaproponuje mu katalog praktyk dopasowanych do potrzeby uzytkownika


2. **Kto ma być użytkownikiem końcowym aplikacji?**

Osoby zainteresowane medytacją, relaksacją, praktykami mindfulness


3. **Czy według Ciebie aplikacja jest user friendly? (Przyjazna dla użytkownika- np. wchodzisz do aplikacji i szybko łapiesz do czego służą przyciski. Poczytaj na ten temat w internecie- co to znaczy, że aplikacja jest przyjazna dla użytkownika)**

Aplikacja jest intuicyjna, łatwo się w niej poruszać. Użytkownik szybko odkrywa funkcje aplikacji. 
Jednak nie do końca zrozumiałem są dla mnie poszczególne obszary na stronie głównej (dla początkujących, Twój cel, Dla Ciebie, Wyzwanie). Nie jest jasne czym się od siebie różnią. 


4. **Jak byś usprawnił aplikację? Co byś w niej poprawił. Czy masz jakiś pomysł na dodatkową funkcjonalność? (Żeby nie było: nie jest to aplikacja przy której pracuję, takie pytania pojawiają się na rozmowach rekrutacyjnych dlatego dobrze jest to przećwiczyć :D )**

Dodałbym funkcję filtrowania praktyk po kryteriach:
* cena
* długość trwania praktyki
* autor
* zrealizowane/niezrealizowane praktyki

Aplikacja ma dużo różnych kategorii - w zakładce Odkrywaj mamy 16 kategorii - prócz tego są w tej samej zakładce inne sekcje - złap oddech, wewnętrzny spokój, ostatnio dodane. Ciężko się w tym odnaleźć. 
Problem jest też zresetowanie postępów praktyk po zmianie języka oraz mniejsza ilość materiału w języku angielskim


5. **Jakie dostrzegasz różnice pomiędzy testowaniem aplikacji internetowej, a natywnej?**

W aplikacji natywnej nie ma devtoolsów, które jednak ułatwiają testowanie i dają inne możliwości
Aplikacje natywne dobrze jest testować na wielu różnych urządzeniach z tej samej grupy (różne telefony, różne tablety). Dodatkowo każde z tych urządzeń może pracować w trybie horyzontalnym i wertykalnym. 
Łatwiej jest mi testować aplikacje webowe, mam wrażenie, że łatwiej jest zrobić to w uporządkowany sposób.

<div id='TASK5'/>

## TASK 5

### Subtask 3
1. Wyświetl tabelę actors w kolejności alfabetycznej sortując po kolumnie surname.

<a href="https://ibb.co/8zn3f69"><img src="https://i.ibb.co/8zn3f69/2023-02-13-19h10-41.png" alt="2023-02-13-19h10-41" border="0" /></a>

2. Wyświetl film, który powstał w 2019 roku.

<a href="https://ibb.co/BfbhXrj"><img src="https://i.ibb.co/BfbhXrj/2023-02-13-19h15-44.png" alt="2023-02-13-19h15-44" border="0" /></a>

3. Wyświetl wszystkie filmy, które powstały między 1900, a 1999 rokiem.

<a href="https://ibb.co/CpLvd9F"><img src="https://i.ibb.co/CpLvd9F/2023-02-13-19h15-04.png" alt="2023-02-13-19h15-04" border="0" /></a>

4. Wyświetl JEDYNIE tytuł i cenę filmów, które kosztują poniżej 7$

<a href="https://ibb.co/7R9pFk2"><img src="https://i.ibb.co/7R9pFk2/2023-02-13-19h17-02.png" alt="2023-02-13-19h17-02" border="0" /></a>

5. Użyj operatora logicznego AND, aby wyświetlić aktorów o actor_id pomiędzy 4-7 (4 i 7 powinny się wyświetlać). NIE UŻYWAJ operatora BETWEEN.

6. Wyświetl klientów o id 2,4,6 wykorzystaj do tego warunek logiczny.

<a href="https://ibb.co/nBcdvnq"><img src="https://i.ibb.co/nBcdvnq/2023-02-13-19h28-57.png" alt="2023-02-13-19h28-57" border="0" /></a>

7. Wyświetl klientów o id 1,3,5 wykorzystaj do tego operator IN.

<a href="https://ibb.co/S7M4T1k"><img src="https://i.ibb.co/S7M4T1k/2023-02-13-19h30-19.png" alt="2023-02-13-19h30-19" border="0" /></a>

8. Wyświetl dane wszystkich osób z tabeli ‘actors’, których imię zaczyna się od ciągu “An”.

<a href="https://ibb.co/k6vWjKv"><img src="https://i.ibb.co/k6vWjKv/2023-02-13-19h32-18.png" alt="2023-02-13-19h32-18" border="0" /></a>

9. Wyświetl dane klienta, który nie ma podanego adresu email.

<a href="https://ibb.co/TB7DTDK"><img src="https://i.ibb.co/TB7DTDK/2023-02-13-19h33-15.png" alt="2023-02-13-19h33-15" border="0" /></a>

10. Wyświetl wszystkie filmy, których cena wynosi powyżej 9$ oraz ich ID mieści się pomiędzy 2 i 8 movie_id.

<a href="https://ibb.co/2W43KX0"><img src="https://i.ibb.co/2W43KX0/2023-02-13-19h34-57.png" alt="2023-02-13-19h34-57" border="0" /></a>



    
