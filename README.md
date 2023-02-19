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
  * IN
  * OR
  * NOT
  * ORDER BY
  * WHERE
  * AND
  * LIKE


 ## Subtask 3
 
  * Wyświetl tabelę actors w kolejności alfabetycznej sortując po kolumnie surname.
  
  SELECT * FROM `actors` ORDER BY `actors`.`surname` ASC
   
   ![1](https://user-images.githubusercontent.com/122168130/218872509-2877d60b-c78d-49a1-ab37-ba308c28c267.png)

  
  * Wyświetl film, który powstał w 2019 roku.
  
  SELECT * FROM `movies` WHERE year_of_production = 2019;
  
  ![2](https://user-images.githubusercontent.com/122168130/218872978-0d9a6b4b-d807-48d6-835c-70962ae16280.png)

  
  * Wyświetl wszystkie filmy, które powstały między 1900, a 1999 rokiem.
  
  SELECT * FROM `movies` WHERE year_of_production between 1900 and 1999;
  
  ![3](https://user-images.githubusercontent.com/122168130/218873070-ab4abe37-ba6b-4c15-aaec-d115dc2cee34.png)


  * Wyświetl JEDYNIE tytuł i cenę filmów, które kosztują poniżej 7$
  
  SELECT `title`,`price` FROM `movies` WHERE `price` <7;
  
  ![4](https://user-images.githubusercontent.com/122168130/218873124-8bd88cb1-9993-49d5-b8e3-253484c26744.png)


  * Użyj operatora logicznego AND, aby wyświetlić aktorów o actor_id pomiędzy 4-7 (4 i 7 powinny się wyświetlać). NIE UŻYWAJ operatora BETWEEN.
  
  SELECT * FROM `actors` WHERE `actor_id` <10 AND (`actor_id`=4 OR `actor_id`=5 OR `actor_id`=6 OR `actor_id`=7);
  
  ![5](https://user-images.githubusercontent.com/122168130/218873176-e02c8822-ce2c-4f7a-9c51-ec36d7bc6fa0.png)


  * Wyświetl klientów o id 2,4,6 wykorzystaj do tego warunek logiczny.
  
  SELECT * FROM `customers` WHERE `customer_id` = 2 OR `customer_id` = 4 OR `customer_id` = 6;
  
  ![6](https://user-images.githubusercontent.com/122168130/218873208-f280dba1-4313-46af-905e-7086d7b7fb84.png)

  
  * Wyświetl klientów o id 1,3,5 wykorzystaj do tego operator IN.
  
  SELECT * FROM `customers` WHERE `customer_id` IN (1, 3, 5)
  
  ![7](https://user-images.githubusercontent.com/122168130/218873249-d48cd9e9-1d48-4ecf-876b-c17a0452a747.png)

  
  * Wyświetl dane wszystkich osób z tabeli ‘actors’, których imię zaczyna się od ciągu “An”.
  
  SELECT * FROM `actors` WHERE `name` LIKE 'An%';
  
  ![8](https://user-images.githubusercontent.com/122168130/218873275-ac68459b-eca5-4e64-95a0-9a65f48afdbd.png)

  
  * Wyświetl dane klienta, który nie ma podanego adresu email.
  
  SELECT * FROM `customers` WHERE `email` IS null;
  
  ![9](https://user-images.githubusercontent.com/122168130/218873319-842b49b5-45b2-4575-87b0-5a6c2bf440d3.png)

  
  * Wyświetl wszystkie filmy, których cena wynosi powyżej 9$ oraz ich ID mieści się pomiędzy 2 i 8 movie_id.
  
  SELECT * FROM `movies` WHERE `price` > 9 AND `movie_id` BETWEEN 2 and 8;
  
  ![10](https://user-images.githubusercontent.com/122168130/218873351-a035227e-bd81-42d8-b3f2-f469fefcac48.png)
  
  # Task 6
  ## Subtask 1
  
  * 11. Popełniłam błąd wpisując nazwisko Ani Miler – wpisałam Muler. Znajdź i zastosuj funkcję, która poprawi mój karkołomny błąd
  
  UPDATE `customers` SET `surname`= 'Miler' WHERE `name`='Ania'
  
  * 12. Pobrałam za dużo pieniędzy od klienta, który kupił w ostatnim czasie film o id 4. Korzystając z funkcji join sprawdź, jak ma na imię klient i jakiego ma maila.
  SELECT *
FROM customers
JOIN sale
ON customers.customer_id =sale.customer_id
WHERE movie_id = 4

SELECT name, email
FROM customers
JOIN sale
ON customers.customer_id =sale.customer_id
WHERE movie_id = 4

  
  
  * 13. Na pewno zauważył_ś, że sprzedawca zapomniał wpisać emaila klientce Patrycji. Uzupełnij ten brak wpisując: pati@mail.com
  
  UPDATE `customers` SET `email`= 'pati@mail.com' WHERE `name`='Patrycja'
  
  * 14. Dla każdego zakupu wyświetl, imię i nazwisko klienta, który dokonał wypożyczenia oraz tytuł wypożyczonego filmu. (wykorzystaj do tego funkcję inner join, zastanów się wcześniej, które tabele Ci się przydadzą do wykonania ćwiczenia).
  
  SELECT movies.title, customers.name, customers.surname FROM sale INNER JOIN movies ON sale.movie_id = movies.movie_id INNER JOIN customers ON sale.customer_id = customers.customer_id;
  
  
  * 15. W celu anonimizacji danych, chcesz stworzyć pseudonimy swoich klientów. - Dodaj kolumnę o nazwie ‘pseudonym’ do tabeli customer,- Wypełnij kolumnę w taki sposób, aby pseudonim stworzył się z dwóch pierwszych liter imienia i ostatniej litery nazwiska. Np. Natalie Pilling → Nag
  
  step 1.
ALTER TABLE customers
ADD pseudonym int

step 2.
UPDATE `customers` 
SET `pseudonym`= 'Ols' WHERE customer_id = 1
UPDATE `customers` 
SET `pseudonym`= 'Kal' WHERE customer_id = 2
UPDATE `customers` 
SET `pseudonym`= 'Anr' WHERE customer_id = 3
UPDATE `customers` 
SET `pseudonym`= 'Par' WHERE customer_id = 4
UPDATE `customers` 
SET `pseudonym`= 'Mao' WHERE customer_id = 5
UPDATE `customers` 
SET `pseudonym`= 'Nag' WHERE customer_id = 6



  
  * 16. Wyświetl tytuły filmów, które zostały zakupione, wyświetl tabelę w taki sposób, aby tytuły się nie powtarzały.
  
  SELECT DISTINCT title
FROM movies
JOIN sale
ON movies.movie_id = sale.movie_id
  
  * 17. Wyświetl wspólną listę imion wszystkich aktorów i klientów, a wynik uporządkuj alfabetycznie. (Wykorzystaj do tego funkcji UNION)
  
  SELECT name
FROM actors 
UNION
SELECT name
FROM customers
ORDER BY name
  
  * 18. Polskę opanowała inflacja i nasz sklepik z filmami również dotknął ten problem. Podnieś cenę wszystkich filmów wyprodukowanych po 2000 roku o 2,5 $ (Pamiętaj, że dolar to domyślna jednostka- nie używaj jej nigdzie).
  
  UPDATE movies SET price = price+2.5 WHERE year_of_production > 2000;
  
  * 19. Wyświetl imię i nazwisko aktora o id 4 i tytuł filmu, w którym zagrał
  
  SELECT actors.name, actors.surname, actors.actor_id, movies.title
FROM cast
JOIN actors ON cast.actor_id = actors.actor_id
JOIN movies ON cast.movie_id = movies.movie_id
HAVING actor_id = 4
  
  * 20. A gdzie nasza HONIA!? Dodaj do tabeli customers nową krotkę, gdzie customer_id = 7, name = Honia, surname = Stuczka-Kucharska, email = honia@mail.com oraz pseudonym = Hoa
  
  INSERT INTO customers (customer_id, email, name, pseudonym, surname) VALUES ('7', 'honia@mail.com', 'Honia', 'Hoa', 'Stuczka-Kucharska')

