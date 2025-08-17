# Skrypt PowerShell: Tworzenie struktury katalogowej z uprawnieniami NTFS.

## Wymagania wstępne

- Maszyna virtualna z systemem _**Windows 11**_.

## Treść zadania

Utwórz dwóch użytkowników lokalnych:
- `Adam`
- `Ewa`

- Napisz skrypt _**powershell**_ który po uruchomieniu utworzy katalog `[nazwa_użytkownika]` w lokalizacji `C:\`.

- Usuń wszystkie uprawnienia i wyłącz *dziedziczenie* na nowo utworzonym katalogu.

- W zależności od tego jaki użytkownik uruchomi skrypt to on ma mieć pełne prawa do katalogu natomiast ten drugi ma mieć odmówione prawo do odczytu.

- Gdy skrypt wykona wszystkie działania to powinien wyświetlić uprawnienia w oknie aplikacji **Terminal**
