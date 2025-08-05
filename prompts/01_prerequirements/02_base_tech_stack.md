Frontend – React z Vite jako nowoczesny, lekki interfejs użytkownika:
- React 19 – popularna, nowoczesna biblioteka komponentów, szeroko wspierana
- Vite – szybki bundler i dev server, idealny dla małych aplikacji i lokalnego developmentu
- Tailwind CSS 4 – nowoczesny, narzędziowy framework CSS umożliwiający szybkie stylowanie
- Shadcn/ui – zestaw gotowych, dostępnych komponentów opartych na Radix UI
- TypeScript 5 – zapewnia silne typowanie i lepszą obsługę przez IDE

Backend – FastAPI jako szybkie i asynchroniczne API do scrapowania danych:
- FastAPI – lekki i szybki framework REST API z automatyczną dokumentacją OpenAPI
- Python 3.12 – nowoczesna wersja Pythona, idealna do pracy z AI, analizą danych i scrapowaniem
- Uvicorn – szybki ASGI server do uruchamiania backendu

Scraping i interpretacja danych:
- FireCrawl – crawler optymalizujący strony do użytku przez LLM, ułatwiający analizę struktury i kontekstu
- BeautifulSoup / Playwright – do klasycznego scrapowania HTML (w zależności od struktury strony)
- pymupdf + Mistral OCR – do ekstrakcji danych technicznych z plików PDF, także ze skanów
- OpenAI LLM (GPT-4.1 lub nowsze) – do interpretacji treści stron i nadawania struktur wyjściowym danym (np. identyfikacja parametrów technicznych, klasyfikacja, rozpoznanie jednostek)
- Dynamiczne modelowanie parametrów produktu – struktura danych budowana w oparciu o zawartość, nie sztywny schemat

CI/CD i uruchamianie lokalne:
- Docker – konteneryzacja backendu, frontendu i scrapera
- Docker Compose – do łatwego uruchamiania aplikacji lokalnie jako kompletnego zestawu usług

Inne cechy:
- Aplikacja nie wymaga logowania – dostęp uproszczony do lokalnego użytku
- Możliwość scrapowania różnych typów stron produktowych, bez potrzeby ich wcześniejszego modelowania
