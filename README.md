# LGOFFB

### Generator offboardingu Google Workspace

Narzędzie dla administratorów IT: formularz w przeglądarce przygotowuje Google Apps Script do uporządkowanego zakończenia dostępu użytkownika.

## Zakres

- Wskazanie konta odchodzącego użytkownika i osoby przejmującej.
- Generowanie nazwy konta archiwalnego i kodu do Apps Script.
- Opcje transferu Drive/Docs i Calendar oraz obsługi starego adresu jako aliasu.
- Opcja usunięcia profilu służbowego z urządzeń Google MDM.
- Instrukcja konfiguracji, uruchomienia i sprawdzenia logów.

## Uruchomienie

1. Pobierz repozytorium i otwórz [index.html](index.html) w przeglądarce.
2. Przejdź przez konfigurację Apps Script opisaną na stronie.
3. Wypełnij formularz i wygeneruj plik `Code.gs`.
4. Pierwsze uruchomienie pozostaw w trybie `EXECUTE: false` (DRY RUN).
5. Sprawdź konta, urządzenia i planowane operacje w logu przed świadomym włączeniem wykonania.

Generator przygotowuje kod; zmiany w środowisku wykonuje dopiero uruchomiony skrypt z odpowiednimi uprawnieniami administratora.

## Ważne ograniczenia

Konto źródłowe jest zawieszane i przemianowywane, nie usuwane. Historyczna poczta pozostaje na koncie archiwalnym; alias dotyczy nowej poczty. Operacja MDM jest przeznaczona do usunięcia konta/profilu służbowego, a nie pełnego resetu urządzenia. Faktyczny zakres operacji zależy od konfiguracji i uprawnień środowiska.

Przed użyciem produkcyjnym sprawdź wygenerowany kod i działanie na kontrolowanym koncie testowym. Dokumentacja opisuje zamierzony przepływ; nie stanowi potwierdzenia testów w Twojej organizacji.

## Technologia

HTML · CSS · JavaScript · Google Apps Script · Google Admin SDK

---

Autor: [Damian Eron](https://github.com/damianx9x) · [Portfolio](https://github.com/damianx9x/damianx9x)
