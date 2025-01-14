# Biblioteka Online
Nasz projekt na GitHub: https://github.com/Natalli09/Biblioteka-Online/tree/master

Projekt Biblioteka Online to system biblioteczny open-source, który umożliwia użytkownikom przeglądanie, wyszukiwanie i dostęp do cyfrowych zasobów, takich jak książki, dokumenty i materiały edukacyjne. Naszym celem jest stworzenie przyjaznego narzędzia, które może być wykorzystywane przez różne organizacje – szkoły, uczelnie czy indywidualnych użytkowników.

## Opis Projektu

Biblioteka Online to aplikacja webowa stworzona w oparciu o PHP, HTML, CSS, JavaScript oraz bazę danych MySQL. Umożliwia ona zarządzanie cyfrową kolekcją książek, zapewniając użytkownikom możliwość przeszukiwania zasobów, pobierania materiałów oraz współdzielenia wiedzy. Projekt obsługuje wiele ról użytkowników, takich jak czytelnicy i administratorzy, z różnymi poziomami dostępu.

## Kluczowe Funkcje:

1. Interfejs użytkownika – intuicyjny i łatwy w obsłudze, zapewniający przyjazne doświadczenie zarówno dla nowych, jak i zaawansowanych użytkowników.
2. System logowania i rejestracji – umożliwia bezpieczne tworzenie kont użytkowników oraz logowanie do systemu, z opcją odzyskiwania zapomnianych haseł.
3. Przesyłanie zasobów – administratorzy mogą dodawać nowe materiały, w tym tytuł, autora, rok wydania, opis, gatunek, oraz inne metadane, w celu pełnego zdefiniowania zasobu.
4. Wyszukiwanie zasobów – użytkownicy mogą przeszukiwać bibliotekę na podstawie różnych kryteriów, takich jak tytuł, autor, gatunek, rok wydania czy oceny użytkowników. Wyszukiwanie wspiera także filtry zaawansowane (np. wg ratingu, dostępności).
5. Panel administratora – interaktywne narzędzie pozwalające administratorom na łatwe zarządzanie zawartością biblioteki, z opcjami edytowania, usuwania oraz dodawania nowych materiałów.
6. Pobieranie plików – użytkownicy mają możliwość zapisania zasobów na urządzeniu lokalnym, by móc je wykorzystać offline.
7. Komentarze – użytkownicy mogą dodawać komentarze do materiałów, dzieląc się opiniami, doświadczeniami i sugestiami, co tworzy interaktywną społeczność.
8. Oceny – użytkownicy mogą oceniać materiały na podstawie własnych doświadczeń, umożliwiając innym użytkownikom łatwiejszą ocenę jakości zasobów na podstawie średniej ocen.
9. Dodawanie do archiwum – możliwość tworzenia list materiałów, które użytkownicy mogą zachować w swoich "archiwach" do późniejszego użytku, zarządzając swoją kolekcją.
10. Podział na gatunki – zasoby są podzielone na kategorie/tematyczne grupy, aby użytkownicy mogli łatwo przeszukiwać bibliotekę według określonego gatunku (np. literackiego, naukowego, edukacyjnego).

## Instalacja

1. Sklonuj repozytorium:

    git clone https://github.com/Natalli09/Biblioteka-Online
    cd online-library

2. Skonfiguruj bazę danych:
    - Utwórz nową bazę danych w MySQL.
    - Zaimportuj plik SQL dostarczony w folderze database/ (np. bookstore.sql) do swojej bazy danych.
    - Skonfiguruj połączenie z bazą danych w pliku config.php.

3. Zainstaluj serwer lokalny:
    - Zainstaluj i uruchom lokalny serwer, taki jak XAMPP, WAMP lub MAMP.
    - Skopiuj pliki projektu do folderu htdocs (lub innego folderu obsługiwanego przez Twój serwer).

4. Uruchom aplikację:
    Otwórz przeglądarkę i przejdź pod adres:
    http://localhost/Biblioteka-Online-master/

## Korzystanie z Aplikacji 
1. Utwórz konto w systemie jako użytkownik biblioteki lub zaloguj się, jeśli już posiadasz konto. 
2. yszukuj książki i dokumenty za pomocą kategorii lub opcji wyszukiwania, aby znaleźć materiały, które Cię interesują. 
3. Możesz czytać książki bezpośrednio w aplikacji albo pobierz książki. 
4. Możesz pisać komentarze i dzielić się swoimi przemyśleniami na temat przeczytanych książek z innymi użytkownikami.Dodaj interesujące Cię książki do archiwum lub listy ulubionych, aby łatwo wrócić do nich w przyszłości. Jako administrator masz możliwość zarządzania zawartością biblioteki, w tym dodawania, edytowania lub usuwania książek.

## Wymagania systemowe

- PHP 7.4 lub nowszy
- MySQL 5.7 lub nowszy
- Serwer lokalny (np. XAMPP, WAMP, MAMP)
- Przeglądarka internetowa

## Struktura projektu

Foldery i ich zawartość:
 admin/
    - add_books.php – Dodawanie nowych książek (dla administratorów).
after_login/
    - edit_profile.php – Edytowanie profilu użytkownika.
    - logout.php – Wylogowanie użytkownika.
    - after_style.css – Stylizacja elementów dostępnych po zalogowaniu.
browser/
    - Zawiera obrazki reprezentujące gatunki książek.
database/
    - bookstore.sql – Plik SQL zawierający schemat bazy danych oraz dane przykładowe.
font-awesome-4.7.0/
    Pliki ikon Font Awesome:
    - css/, fonts/, less/, scss/ – Foldery potrzebne do wyświetlania ikon.
hdimg/
    Grafiki interfejsu:
    - homeback.png – Tło strony głównej.
    - logo.png – Logo aplikacji.
uploads/
    Folder na przesyłane pliki, np. zdjęcia profilowe użytkowników i okładki książek.

Pliki w katalogu głównym:
- index.php – Strona główna systemu biblioteki.
- signup.php – Formularz rejestracji nowych użytkowników.
- profile.php – Strona profilu użytkownika z możliwością edycji.
- delete_book.php – Usuwanie książek z bazy danych.
- edit_book.php – Edytowanie szczegółów książek.
- search.php – Wyszukiwanie książek.
- readBook.php – Czytanie książek online.
- genre.php – Wyświetlanie książek według gatunku.
- ebook_style.css – Stylizacja sekcji e-booków.
- LICENSE – Informacje o licencji projektu.
