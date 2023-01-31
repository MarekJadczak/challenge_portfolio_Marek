# challenge_portfolio_Marek

## SPIS TREŚCI
1. [TASK 1](#TASK1)

2. [TASK 2](#TASK2)

3. [TASK 3](#TASK3)

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
    
