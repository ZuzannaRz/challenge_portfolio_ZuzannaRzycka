# Task 1
## Subtask 1
5 punktów
## Subtask 3
Cześć! Jestem Zuza i zdecydowałąm się wziąć udziałw wyzwaniu aby rozpocząć nową ścieżkę kariery w życiu. Chciałabym uczyć się dobrych praktyk od podstaw oraz stworzyć portfolio, które pozwoli przyszłemy pracodawcy wybrać właśnie mnie.
## Subtask 4
* aplikacja służy do katalogowania graczy, zarządzania ich profilami oraz generowania raportów.

* funkcjonalności aplikacji: 
  * zalogowanie/wylogowanie
  * dodanie nowego gracza i wprowadzenie jego indywidualnych parametrów
  * generwanie bazy graczy w formie tabeli
  * drukowanie bazy graczy
  * wyświetlanie bazy graczy używając kryteriów: imię/nazwisko/wiek/pozycja/klub/recenzja/mecze/raporty
  * filtrowanie bazy graczy używając kryterów: imię/nazwisko/wiek (zakres)/ pozycja/klub/ ranking(zakres)
  * wyświetla niezapisany mecz na "stronie głównej"
  * pokazuje ostatnie atywności: ostatnio stworzony gracz, ostatnio zaktualizowany gracz, ostatnio stworzony mecz, ostatnio zaktualizowany mecz, ostatnio zaktualizowany raport na "stronie głównej"
  * podsumowuje ilość graczy, ilośc meczy, ilośc raportów i ilość akcji na "stronie głównej"
  * generuje listę zdarzeń dla zawodnika z akji które działy się w danym meczu
  * umożliwia generowanie raportów z meczu dla zawodnika
  * tworzy statystykę (wykres słupkowy) podań dla zawodnika

* interfejs aplikacji jest prosty i przejrzysty bez zbędnych elementów, dobrze się w nim porusza.

* panel główny jest intuicyjny, ale dodanie meczu lub raportu danego gracza trzeba chwilę poszukać


* moim zdaniem warto byłoby poprawić:
  * wejście w panel konkretnego zawodnika za pomocą przycisku akcji zamiast dwukrotnego kliknięcia
  * ujednolicenie języka (np. w filtrowaniu rate zamiast recenzja)
  * system dopuszcza parametry ujemne (wiem, wzrost, waga zawodnika)
  * można dodać gracza tylko z poziomu "strony głównej", dobrze byłoby móc to zrobić z poziomu bazy graczy
  * rozpoczęcie meczu (rozegranie go) jest niemożliwe do przeprowadzenia bez objaśnień

 * błędy znalezione przy użyciu DevTools:
  * DevTools failed to load source map: Could not load content for chrome-extension://cfhdojbkjhnklbpkdaibdccddilifddb/browser-polyfill.js.map: System error: net::ERR_FILE_NOT_FOUND 
  * Uncaught (in promise) Error: The provided `as` value (/pl/players/6026b48956c79737b3f3c624/reports/start) is incompatible with the `href` value (/players/[id]/reports/start). Read more: https://err.sh/vercel/next.js/incompatible-href-as     przy próbie powrotu do raportu niezapisanego meczu
  * Params `start` and `limit` are deprecated. Use `_start` and `_limit`   po otwarciu zakładki "gracze"
  * DevTools failed to load source map: Could not load content for chrome-extension://cfhdojbkjhnklbpkdaibdccddilifddb/browser-polyfill.js.map: System error: net::ERR_FILE_NOT_FOUND   zakłądka gracze, po kliknięciu "print"
  * DevTools failed to load source map: Could not load content for chrome-extension://cfhdojbkjhnklbpkdaibdccddilifddb/browser-polyfill.js.map: System error: net::ERR_FILE_NOT_FOUND  po wejściu w szczegóły dowolnego gracza w zakładce gracze


# Task 2

[Link do dysku Google](https://drive.google.com/drive/folders/1m5DYhsqjTcRLIZXE9gPDTh7DB3eXJjcT?usp=share_link)

## Subtask 3 
Po co piszemy test case'y?
Przypadki testowe piszemy, aby udokumentować różne możliwości obsługi aplikacji. Można je wykorzystać w kontekście testów akceptacyjnych oceniając czy aplikacja spełnia wymagania. Są też dobrym źródłem informacji o aplikacji dl aosób wdrażających się w jej testowanie.

# Task 3

## Subtask 1, 2, 3

[Link do dysku Google](https://drive.google.com/drive/folders/1Un6t04ALf7bs39GwqEMM_z1gGPhHQINE?usp=sharing)

# Task 4

## Subtask 1, 2 
[Link do dysku Google](https://docs.google.com/document/d/1720lPG4xdjJ9dxdsneL5RQAbqlXD1hmMKAQ6MGfjKdU/edit?usp=share_link)

## Subtask 3
 * Do czego służy ta aplikacja? 
 do kupowania oraz sprzedawania rzeczy, są na niej publikowane ogłoszenia dotyczące najmu np nieruchomości, wynajmu okresowego rzeczy oraz pracy.
 
 * Jaki jest cel tej aplikacji?
 aplikacja ma na celu gromadzenie ogłoszeń kupna/sprzedaży
 
 * Kto ma być użytkownikiem końcowym aplikacji?
 kupujący lub poszukujący usług
 
 * Czy według Ciebie aplikacja jest user friendly? 
 tak
 
 * Jak byś usprawnił aplikację? Co byś w niej poprawił. Czy masz jakiś pomysł na dodatkową funkcjonalność? 
 głównym minusem, jest przekierowanie procesu rejestracji/logowania do przeglądarki 
 
 * Jakie dostrzegasz różnice pomiędzy testowaniem aplikacji internetowej, a natywnej?
 moim zdaniem testowanie aplikacji natywnej jest dużo szybsze
 
 # Task 5
 ## Subtask 1
  * SELECT * FROM (nazwa tabeli)
  * USE (nazwa bazy danych)


 ## Subtask 3
 
  * Wyświetl tabelę actors w kolejności alfabetycznej sortując po kolumnie surname.
  
  SELECT * FROM `actors` ORDER BY `actors`.`surname` ASC
  
  * Wyświetl film, który powstał w 2019 roku.
  
  SELECT * FROM `movies` WHERE year_of_production = 2019;
  
  * Wyświetl wszystkie filmy, które powstały między 1900, a 1999 rokiem.
  
  SELECT * FROM `movies` WHERE year_of_production between 1900 and 1999;

  * Wyświetl JEDYNIE tytuł i cenę filmów, które kosztują poniżej 7$
  
  SELECT `title`,`price` FROM `movies` WHERE `price` <7;

  * Użyj operatora logicznego AND, aby wyświetlić aktorów o actor_id pomiędzy 4-7 (4 i 7 powinny się wyświetlać). NIE UŻYWAJ operatora BETWEEN.
  
  SELECT * FROM `actors` WHERE `actor_id` <10 AND (`actor_id`=4 OR `actor_id`=5 OR `actor_id`=6 OR `actor_id`=7);

  * Wyświetl klientów o id 2,4,6 wykorzystaj do tego warunek logiczny.
  
  SELECT * FROM `customers` WHERE `customer_id` = 2 OR `customer_id` = 4 OR `customer_id` = 6;
  
  * Wyświetl klientów o id 1,3,5 wykorzystaj do tego operator IN.
  
  SELECT * FROM `customers` WHERE `customer_id` IN (1, 3, 5)
  
  * Wyświetl dane wszystkich osób z tabeli ‘actors’, których imię zaczyna się od ciągu “An”.
  
  SELECT * FROM `actors` WHERE `name` LIKE 'An%';
  
  * Wyświetl dane klienta, który nie ma podanego adresu email.
  
  SELECT * FROM `customers` WHERE `email` IS null;
  
  * Wyświetl wszystkie filmy, których cena wynosi powyżej 9$ oraz ich ID mieści się pomiędzy 2 i 8 movie_id.
  
  SELECT * FROM `movies` WHERE `price` > 9 AND `movie_id` BETWEEN 2 and 8;
