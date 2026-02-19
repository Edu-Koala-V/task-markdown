# Udział plików i folderów Samba

## Wymagania wstępne

- Maszyna virtualna z systemem _**Ubuntu Server 24.04**_.
- Maszyna virtualna z systemem _**Windows 11 Pro**_.
- Maszyna virtualna z systemem _**Ubuntu Desktop 24.04**_.

## Treść zadania

- Skonfiguruj usługę sieciową `Samba` na serwerze i pamiętaj o ustawieniu `SMB v3.0` lub nowszej, bo _**Windows 11**_ Pro nie będzie się chciał połączyć z niższą wersją protokołu.
- Utwórz użytkownika `Lucek` i trzy udziały:

| Udział      |  Zapis  |  Odczyt | Dostęp bez logowania |
| :---------- | :-----: | :-----: | -------------------: |
| publiczne   | **NIE** | **TAK** |              **TAK** |
| prywatne    | **NIE** | **TAK** |        tylko _Lucek_ |
| lucka_pliki | **TAK** | **TAK** |        tylko _Lucek_ |

## Wynik

- publiczne - dostępny dla wszystkich, ale tylko do odczytu
- prywatne - dostępny tylko dla użytkownika _Lucek_, ale tylko do odczytu
- lucka_pliki - pełny dostęp (zapis i odczyt) tylko dla użytkownika _Lucek_
