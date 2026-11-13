# Lietuvių B1: litewski 10 minut dziennie

Samodzielna aplikacja do codziennej nauki litewskiego na poziomie **B1** dla osób mówiących po polsku.
To **jeden plik `index.html`**. Działa w każdej przeglądarce (telefon, tablet, komputer), także **bez internetu**.
Nie potrzebuje konta, subskrypcji (np. Claude Pro) ani żadnych opłat.

## Jak zacząć
1. Skopiuj plik `index.html` na telefon lub komputer (mailem, przez Dysk Google, WhatsApp…).
2. Otwórz go w przeglądarce (Chrome, Safari, Firefox).
3. Na telefonie: menu przeglądarki → **„Dodaj do ekranu głównego”**, żeby mieć ikonkę jak aplikację.

> Postępy zapisują się w tej przeglądarce, na tym urządzeniu. Raz na jakiś czas warto zrobić
> **Ustawienia → Zapisz kopię** (plik `.json`), żeby można było przenieść postępy na inne urządzenie.

## Co jest w środku
| Część | Co robi |
|---|---|
| **Codzienna lekcja (10 min)** | powtórki słówek → nowe słowa → przypomnienie zasady → ćwiczenia z gramatyki → poprawianie zdań → utrwalenie nowych słów. Zegar pilnuje 10 minut. |
| **Słówka** | ~250 słów B1 w tematach (zdrowie, podróże, urzędy, praca, opinie…). Ćwiczenia: wybór znaczenia, wybór słowa litewskiego, wpisywanie. Przyciski z literami ą č ę ė į š ų ū ž. |
| **Gramatyka** | 17 tematów (przypadki, czasy, tryb przypuszczający i rozkazujący, czasowniki zwrotne, stopniowanie, liczebniki, imiesłowy, przyimki, spójniki, *savo*). Krótkie ściągi po polsku z tabelkami. |
| **Poprawianie zdań** | zdania z typowymi błędami Polaków (np. *važiuoju **su** autobusu*, *aš turiu 60 metų*, *einu į gydytoją*). Do wyboru albo do samodzielnej poprawy, z wyjaśnieniem. |
| **Powtórki rozłożone w czasie** | algorytm SM-2: co trudne, wraca szybciej; co łatwe, wraca coraz rzadziej (1 → 3 → 7 → 20+ dni). Błędna odpowiedź wraca jeszcze w tej samej lekcji. |
| **Poziom adaptacyjny** | co 6 odpowiedzi program patrzy na ostatnie 10: przy ≥85% podnosi poziom (więcej wpisywania, trudniejszy materiał B1+), przy ≤55% obniża (więcej wyboru, łatwiejsze rzeczy, mniej nowych słów). Słabsze tematy gramatyki pojawiają się częściej. |
| **Notatnik** | własne notatki, przycisk „📒 Do notatnika” przy błędach, lista trudnych słów, ostatnie błędy, wyszukiwarka poznanych słów. |
| **Statystyki** | seria dni 🔥, minuty, skuteczność (słówka, gramatyka, zdania, każdy temat), słowa opanowane, kalendarz aktywności, wykres poziomu, prognoza powtórek. |
| **Lektor 🔊** | czyta słowa po litewsku, jeśli urządzenie ma litewski głos (Ustawienia pokazują, czy jest). |

## Jak dodać własne słowa / ćwiczenia
W `index.html` znajdziesz na górze sekcje danych:
- `VOCAB_TXT`: linie `litewski = polski` pod nagłówkiem `#poziom Temat` (1 = B1 podstawa, 2 = B1, 3 = B1+),
- `GRAM_RAW`: ćwiczenia z luką: `[temat, poziom, "zdanie z ___", "podpowiedź", "odpowiedź|wariant", "zła1|zła2|zła3", "tłumaczenie"]`,
- `SENT_RAW`: zdania z błędem: `[poziom, temat, "zdanie z błędem", "poprawne|inny poprawny wariant", "inna błędna wersja", "tłumaczenie", "wyjaśnienie"]`.
