# Zarządzanie użytkownikami i grupami lokalnymi
## Wymagania wstępne
- Maszyna wirtualna z systemem **Windows 11 Pro**, **Enterprise** lub **Education**.
- Zainstalowany **PowerShell ISE**.
- Polityka wykonywania skryptów ustawiona na **`RemoteSigned`**.
## Treść zadania
- Uruchom **PowerShell ISE** jako administrator.
- Napisz skrypt **PowerShell** o nazwie "**`ZarządzajUzytkownikami.ps1`**", który wykona następujące operacje:
    - Utwórz nowego użytkownika lokalnego o nazwie "**`AdminSzkolny`**" z hasłem "**`SuperBezpieczne!123`**". Upewnij się, że używasz **`ConvertTo-SecureString`** do bezpiecznego formatowania hasła.
    - Utwórz nową grupę lokalną o nazwie "**`NauczycieleIT`**".
    - Dodaj użytkownika "**`AdminSzkolny`**" do grupy "**`NauczycieleIT`**".
    - **Dodaj użytkownika "**`AdminSzkolny`**" do grupy "**`Użytkownicy`**", aby mógł zalogować się przez interfejs graficzny (GUI)**.
    - Dodaj użytkownika "**`AdminSzkolny`**" do grupy "**`Administratorzy`**".
    - Wyświetl informacje o utworzonym użytkowniku i grupie, aby zweryfikować ich istnienie (użyj `Get-LocalUser` i `Get-LocalGroup`).
- Uruchom skrypt i **zweryfikuj** utworzenie użytkownika i grup w przystawce _lusrmgr.msc_. Spróbuj zalogować się na konto `AdminSzkolny`.
