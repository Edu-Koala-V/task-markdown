# Skrypt PowerShell: Kreator udziałów sieciowych na nowym dysku

## Wymagania wstępne

- Maszyna virtualna z systemem _**Windows 11**_.

## Treść zadania

- Dodaj nowy dysk **SATA** ($$2GB$$) do maszyny z _**Windows 11**_.

- Utwórz użytkownika lokalnego: `Marek`

- Napisz skrypt _**powershell**_ który:
  
  - po uruchomieniu sprawdzi czy w systemie są co najmniej $$2$$ dyski.

  - Przetworzy dodatkowy dysk na wolumin **_GPT_** z literą `M`

  - Na nowym woluminie utworzy się katalog `katalog_share\`.

  - Utworzy udział sieciowy z lokalizacji `M:\katalog_share\` dla użytkownika `Marek` 
