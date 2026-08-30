# a11y-plan

## Cel projektu
Zwiększenie dostępności strony, poprawa czytelności i komfortu użytkowania dla osób korzystających z klawiatury, czytników ekranu, urządzeń mobilnych oraz osób z ograniczeniami wzroku i percepcji.

## Opis zadań projektu

### 1. Semantyka i struktura dokumentu
- [ ] Sprawdzić poprawność użycia nagłówków: `h1`, `h2`, `h3` itd.
- [ ] Uporządkować znaczenie sekcji strony (`header`, `nav`, `main`, `footer`).
- [ ] Upewnić się, że listy i linki są semantycznie prawidłowe.
- [ ] Dodać opisowe nazwy elementów interaktywnych, w tym menu i przyciski zmiany języka.

### 2. Nawigacja klawiaturowa
- [ ] Umożliwić przechodzenie po wszystkich interaktywnych elementach przy użyciu klawiatury.
- [ ] Dodać obsługę `Tab`, `Enter`, `Space` i strzałek w menu rozwijanych.
- [ ] Ustawić widoczny stan focus dla przycisków, linków i elementów listy.
- [ ] Upewnić się, że rozwijane menu zamykają się poprawnie po zmianie aktywnego elementu.

### 3. Dostępność wizualna
- [ ] Dodać style `:focus` i `:focus-visible` do wszystkich aktywnych elementów.
- [ ] Zwiększyć kontrast tekstu względem tła.
- [ ] Sprawdzić czytelność na mobilnych ekranach i w małych rozmiarach tekstu.
- [ ] Upewnić się, że ważne elementy nie są ukryte tylko przez kolor lub przez opacity.

### 4. Media, dźwięk i animacje
- [ ] Dodać nazwy i opisy dla obrazów, GIF-ów i wideo.
- [ ] Zabezpieczyć automatyczne odtwarzanie dźwięku przed użytkownikiem.
- [ ] Dodać możliwość wyciszenia/wyłączenia efektów dźwiękowych.
- [ ] Upewnić się, że animacje nie utrudniają czytania treści ani nie migają zbyt intensywnie.

### 5. Responsywność i układ
- [ ] Przejrzeć układ menu i stopki pod kątem nakładania się elementów.
- [ ] Ujednolicić nazewnictwo klas i poprawić czytelność CSS.
- [ ] Dodać poprawne zachowanie na różnych szerokościach ekranów.
- [ ] Weryfikować, czy tekst i przyciski nie są zbyt małe lub zbyt ciasne.

### 6. Testowanie i walidacja
- [ ] Przejść po stronie wyłącznie klawiaturą.
- [ ] Sprawdzić kolejność focusu i przejście między sekcjami.
- [ ] Uruchomić testy dostępności w Lighthouse / axe / WAVE.
- [ ] Przetestować podstawową obsługę czytnikiem ekranu.
- [ ] Zweryfikować kontrast i czytelność po zmianach.

### 7. Refaktoryzacja i porządek kodu
- [ ] Usunąć zbędny, nieużywany kod JavaScript.
- [ ] Ujednolicić nazwy zmiennych i funkcji.
- [ ] Uporządkować style CSS, aby łatwiej było je rozbudowywać.
- [ ] Zachować spójność między HTML, CSS i JavaScript.

## Checklista sprintowa

### Sprint 1 – podstawy dostępności i intuicyjnej nawigacji
- [ ] Przejrzeć i poprawić semantykę HTML w sekcjach `nav`, `header`, `main`, `footer`
- [ ] Dodać widoczny stan `:focus` i `:focus-visible` dla wszystkich linków, przycisków i elementów list rozwijanych
- [ ] Umożliwić pełną obsługę strony z klawiatury (Tab, Enter, Spacja, Strzałki)
- [ ] Zapewnić działanie menu rozwijanych bez myszki
- [ ] Dodać tekstowe etykiety/label dla elementów interaktywnych i dynamicznych list
- [ ] Sprawdzić, czy wszystkie elementy mają logiczną kolejność fokusowania
- [ ] Przeprowadzić testy ręczne z klawiatury i wstępny audit Lighthouse

### Sprint 2 – dostępność wizualna i czytelność
- [ ] Zwiększyć kontrast tekstu i elementów interaktywnych
- [ ] Poprawić czytelność na małych ekranach i przy zmniejszonym zoomie
- [ ] Uporządkować układ menu, hintów i stopki, aby nie nakładały się na siebie
- [ ] Ujednolicić nazewnictwo klas i usunąć zbędne duplikaty CSS
- [ ] Dodać poprawne zachowanie dla hover/focus w menu i przyciskach
- [ ] Zweryfikować, czy ważne informacje nie zależą wyłącznie od koloru

### Sprint 3 – multimedia, dźwięk i animacje
- [ ] Dodać opisy dla obrazów, GIF-ów i wideo
- [ ] Zabezpieczyć automatyczne odtwarzanie audio i wideo
- [ ] Dodać możliwość wyciszenia / zatrzymania efektów dźwiękowych
- [ ] Ustawić sensowne ograniczenia dla animacji i efektów ruchu
- [ ] Sprawdzić, czy animacje nie utrudniają czytania treści ani nie powodują dyskomfortu

### Sprint 4 – testy, walidacja i porządek kodu
- [ ] Przetestować główne scenariusze użytkownika z czytnikiem ekranu
- [ ] Uruchomić testy dostępności w narzędziach typu Lighthouse, axe, WAVE
- [ ] Wprowadzić poprawki wynikające z audytu
- [ ] Usunąć nieużywane fragmenty JavaScript i zduplikowane reguły CSS
- [ ] Zrobić finalny przegląd strony pod kątem spójności i użyteczności

### Priorytety według pilności
- [ ] P0: focus, klawiatura, semantyka, etykiety
- [ ] P1: kontrast, responsywność, układ
- [ ] P2: media, dźwięk, animacje
- [ ] P3: refaktoryzacja i finalna walidacja

## Główne luki a11y do poprawy
- Brak pełnej obsługi klawiatury w menu rozwijanych.
- Brak widocznego fokusa dla aktywnych elementów.
- Brak `aria-*` lub właściwych etykiet dla dynamicznych elementów.
- Brak opisów dla multimediów i dźwięków.
- Automatyczne efekty mogą przeszkadzać użytkownikom.
- Brak pełnej walidacji dostępności narzędziami automatycznymi.
- Wymagana weryfikacja kontrastu i czytelności na małych ekranach.

## Kolejność wdrażania
1. Poprawa dostępu klawiaturowego i focus.
2. Semantyka HTML i etykiety.
3. Animacje, dźwięk i media.
4. Responsywność i kontrast.
5. Testy i finalna weryfikacja.

## Wskazówka
Najpierw poprawić dostępność funkcjonalną, a dopiero potem estetykę. To daje największą poprawę użyteczności dla użytkowników i minimalizuje ryzyko błędów w działaniu strony.
