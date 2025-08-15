# Interfejsy sieciowe Ubuntu Server - Ubuntu Klient

## Wymagania wstępne

- Maszyna virtualna z systemem _**Ubuntu 24.04 Desktop**_.
- Maszyna virtualna z systemem _**Ubuntu 24.04 Server**_.

## Treść zadania

- Skonfiguruj ustawienia maszyn virtualnych:
  - _**Ubuntu 24.04 Desktop**_:
    - **Karta 2**: `NAT`.
    - **Karta 3**: `Sieć wewnętrzna`.
  - _**Ubuntu 24.04 Server**_:
    - **Karta 1**: `Sieć wewnętrzna`.

- Dokonaj konfiguracji interfejsów sieciowych działających w trybie `Sieć wewnętrzna`.

    | _**Ubuntu 24.04 Server**_ |                      |
    | ------------------------- | -------------------- |
    | Adres IP                  | `10.0.5.20/16`       |
    | Adresy DNS                | `8.8.4.4`, `1.1.1.1` |
    
    | _**Ubuntu 24.04 Desktop**_ |                    |
    | -------------------------- | ------------------ |
    | Adres IP                   | `10.0.10.30/16`     |
    | Adres bramy domyślnej      | `Adres IP Servera` |
    | Adresy DNS                 | `Adres IP Servera` |

- Przeprowadź test łączności komendą `ping` pomiędzy maszynami.
