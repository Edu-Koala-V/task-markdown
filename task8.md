# PowerShell: Kontrola dostępu NTFS na plikach i folderach
## Wymagania wstępne
- Maszyna wirtualna z systemem **Windows 11 Pro**, **Enterprise** lub **Education**.
- Zainstalowany **PowerShell ISE**.
- Utwórz dwóch użytkowników: **`UzytkownikA`** i **`UzytkownikB`**.
- Utwórz folder testowy o nazwie `C:\ProjektDanych`. W nim utwórz plik `tajny_raport.txt` i napisz w nim coś.
## Treść zadania
- Uruchom **PowerShell ISE** jako administrator.
- Napisz skrypt **PowerShell**, który wykona następujące operacje na folderze `C:\ProjektDanych` i pliku `tajny_raport.txt`:
    - Użyj **`Get-Acl`** do wyświetlenia bieżących uprawnień folderu `C:\ProjektDanych`. Zapisz je do zmiennej.
    - **Dodaj regułę `Deny`** dla użytkownika **`UzytkownikA`** z uprawnieniem **`ReadAndExecute`** dla folderu `C:\ProjektDanych`. Upewnij się, że reguła dziedziczy się na podfoldery i pliki (`ContainerInherit`, `ObjectInherit`).
    - **Dodaj regułę `Allow`** dla użytkownika **`UzytkownikB`** z uprawnieniem **`Modify`** dla folderu `C:\ProjektDanych`.
    - **Wyjaśnij i zademonstruj zasadę "Deny ma większy priorytet niż Allow"**:
        - Spróbuj zalogować się na konto `UzytkownikA` i `UzytkownikB`.
        - Jako `UzytkownikA` spróbuj odczytać zawartość `tajny_raport.txt` i opisz, co się dzieje.
        - Jako `UzytkownikB` spróbuj zmodyfikować `tajny_raport.txt`.
    - Usuń regułę `Deny` dla użytkownika `UzytkownikA`.
    - **Wyłącz dziedziczenie uprawnień** dla folderu `C:\ProjektDanych` za pomocą `SetAccessRuleProtection`, zachowując dotychczasowe uprawnienia jako jawne.
