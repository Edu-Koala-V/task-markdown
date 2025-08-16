# PowerShell Scripting: Interaktywne narzędzie diagnostyczne sieci
## Wymagania wstępne
- Maszyna wirtualna z systemem **Windows 11**.
- Zainstalowany **PowerShell ISE**.
- Polityka wykonywania skryptów ustawiona na **`RemoteSigned`**.
## Treść zadania
- Uruchom **PowerShell ISE** jako administrator.
- Napisz interaktywny skrypt **PowerShell**, który będzie służył do podstawowej diagnostyki sieci. Skrypt powinien:
    - Wyświetlić menu z opcjami:
        1.  `ipconfig /all` (wyświetlenie pełnej konfiguracji sieciowej).
        2.  `ping` (testowanie łączności z adresem IP/nazwą hosta).
        3.  `nslookup` (zapytanie DNS o adres IP domeny).
        4.  `netstat -aon` (wyświetlenie aktywnych połączeń i nasłuchujących portów z PID).
        5.  Wyjście.
    - Użyj pętli **`while`**, aby menu wyświetlało się tak długo, aż użytkownik nie wybierze opcji wyjścia.
    - Użyj **`Read-Host`** do pobrania wyboru użytkownika.
    - Użyj instrukcji **`switch`**, aby wykonać odpowiednie polecenie w zależności od wyboru użytkownika:
        - Dla `ipconfig /all` i `netstat -aon`, po prostu wykonaj komendę.
        - Dla `ping`: zapytaj użytkownika o adres IP lub nazwę hosta do spingowania.
        - Dla `nslookup`: zapytaj użytkownika o nazwę domeny.
    - Zaimplementuj **obsługę błędów** za pomocą bloku **`try-catch`** dla operacji sieciowych (np. gdy ping nie znajdzie hosta lub nslookup nie rozwiąże nazwy). Użyj **`Write-Error`** do wyświetlania komunikatów o błędach. **Pamiętaj o `-ErrorAction Stop` dla poleceń, które domyślnie generują błędy nieterminujące**.
- Po każdym wykonanym poleceniu, skrypt powinien poczekać na naciśnięcie Enter, zanim wróci do menu.
