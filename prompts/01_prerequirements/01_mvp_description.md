### Główny problem
Architekci i projektanci wnętrz spędzają dużo czasu na ręcznym przeszukiwaniu stron producentów w poszukiwaniu informacji o produktach — takich jak drzwi, okna, podłogi itd. Obecnie dostępne aplikacje, które umożliwiają przeszukiwanie produktów, rzadko pozwalają na filtrowanie po konkretnych parametrach technicznych. Dodatkowo, informacje są często rozproszone, ukryte w różnych sekcjach stron lub zawarte w plikach PDF.

Brakuje narzędzia, które umożliwiałoby użytkownikowi szybkie podanie adresu URL strony produktu, a następnie automatyczne wyciągnięcie istotnych danych i zaprezentowanie ich w jednolitej, przystępnej formie.

### Najmniejszy zestaw funkcjonalności (MVP)
- Prosty interfejs webowy, w którym użytkownik podaje URL strony produktu (np. ze strony producenta)
- Backend w Pythonie scrapuje stronę i:
  - przechodzi po jej strukturze, aby zidentyfikować sekcje produktowe
  - automatycznie identyfikuje i wyciąga parametry techniczne (np. wymiary, kolory, klasy ogniowe), które są dopasowywane dynamicznie na podstawie zawartości strony — bez z góry zdefiniowanej struktury
  - pobiera dodatkowe dane: nazwa produktu, opisy, zdjęcia, pliki do pobrania
  - w przypadku, gdy dane znajdują się w plikach PDF, parser próbuje również je zidentyfikować i wydobyć odpowiednie informacje
- Frontend wyświetla dane w czytelnej, ustrukturyzowanej formie (np. lista parametrów, opisy, załączniki)
- Aplikacja obsługuje różne typy stron produktowych i potrafi adaptować się do różnych struktur HTML

### Co NIE wchodzi w zakres MVP
- Automatyczne scrapowanie całych katalogów lub wielu stron naraz
- Zaawansowany system użytkowników i uwierzytelnianie
- Eksporty danych (np. CSV, integracje z CAD/BIM)
- Hosting produkcyjny
- Rozbudowane filtrowanie, przeszukiwanie po parametrach
- Przetrzymywanie wyników w bazie danych

### Kryteria sukcesu
- Użytkownik może podać link do strony produktu i w krótkim czasie uzyskać kluczowe informacje w jednolitym widoku
- Dane wyciągnięte ze strony (i ewentualnie z plików PDF) są zrozumiałe i przydatne dla architekta lub projektanta
- Aplikacja działa stabilnie i poprawnie identyfikuje dane na różnych typach stron producentów

