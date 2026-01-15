# 2. Techniki tworzenia aplikacji typu Single Page Application.

|SPA|MPA|
|---|---|
| Jednostronnicowa aplikacja internetowa | Wielostronnicowa aplikacja internetowa |
| Jeden plik HTML pobierany przy pierwszym załadowaniu strony| Wiele plików HTML każdy jest generowany i ładowany przez back-end podczas zmiany podstrony |
| Strona renderowana po stronie użytkownika| Strona renderowana przez serwer|
| Brak efektu przeładowania strony (wszystko renderowane przez JS) | Przeładowanie strony przy każdej zmianie komponentu |
| Niezbedność mechanizmu AJAX, zezwalający na asynchroniczne pobieranie danych z np. bazy danych |  |
| Szybkie ładowanie strony | długi czas ładowania |
| Słabe wsparcie SEO  | Dobre wsparcie SEO |

### Co by się stało, gdyby dane były pobierane synchronicznie?
Jeśli SPA działałoby synchronicznie, każda prośba o dane powodowałaby tzw. blokowanie wątku głównego (Main Thread).

##### Zamrożenie GUI:
Przeglądarka używa jednego wątku do obsługi JavaScriptu oraz renderowania interfejsu. Pobieranie synchroniczne "zatrzymuje czas" dla przeglądarki. Dopóki serwer nie odpowie, użytkownik nie może kliknąć niczego na stronie, a animacje (np. kręcący się spinner) zostaną zatrzymane w bezruchu.

### Kiedy warto użyć SPA?

Budujesz narzędzie, które wymaga wielu interakcji (np. edytor, dashboard).	
Zależy Ci na płynnych animacjach i przejściach.	
Chcesz mieć wspólne API dla webu i mobile.

### Aplikacje PWA (Progressive Web App)
aplikacja internetowa uruchamiana tak jak zwykła strona internetowa, ale działająca podobnie jak natywna aplikacja mobilna, spójna interfejsem, wrażeniami z korzystania oraz funkcjonalnościami. Powinna być w stanie działąć w pewnym stopniu offline. W dużym skrócie jest to instalowalna strona internetowa. Wymogi dla aplikacji PWA
- szybkie działąnie i zoptymalizowana ilość przesłanych danych
- Poprawne wyświetlanie się na każdym medium
- Dostosowany wygląd (natywny na urządzeniach) i zachowanie (np gesty na aplikacjach mobilnych)
- Możliwość pracy w warunkach offline.
- Dane aktualizują się w tle

## Streszczenie
- SPA vs MPA
- SEO wytłumaczenie o co cho
- Wykorzystanie SPA w dzisiejszym świecie
