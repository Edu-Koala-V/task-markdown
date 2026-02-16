# DHCP Linux z rezerwacją adresu IP

## Wymagania wstępne

- Maszyna virtualna z systemem _**Ubuntu 24.04 Desktop**_.
- Maszyna virtualna z systemem _**Ubuntu 24.04 Server**_.
- Maszyna virtualna z systemem _**Windows 11**_.

## Treść zadania



- Dokonaj konfiguracji DHCP na serwerze _**Ubuntu 24.04 Server**_ tak, aby przydzielał adresy IP z zakresu `192.168.0.50 - 192.168.0.60`.
- Skonfiguruj rezerwację adresu IP `192.168.0.69` dla systemu _**Windows 11**_.

Wynik konfiguracji powinien być następujący:

| System operacyjny          | Adres IP     |
| ------------------------- | ------------ |
| _**Ubuntu 24.04 Server**_ | `192.168.0.11/24` |
| _**Ubuntu 24.04 Desktop**_ | `192.168.0.50/24` (Pierwszy z puli DHCP) |
| _**Windows 11**_          | `192.168.0.69/24` |

- Przeprowadź test łączności komendą `ping` pomiędzy maszynami.
