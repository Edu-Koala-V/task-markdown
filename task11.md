# Windows Serwer - Konfiguracja DNS z aliasami

## Wymagania wstępne

- Maszyna virtualna z systemem _**Windows Server 2025**_.
- Maszyna virtualna z systemem _**Ubuntu 24.04 Desktop**_.
- Maszyna virtualna z systemem _**Windows 11 Pro**_.

Każda maszyna powinna mieć po dwie karty sieciowe (`NAT` i `sieć wewnętrzna`).

## Treść zadania


- Dokonaj konfiguracji wyszukiwania do przodu i do tyłu *DNS* na adres serwera z nazwą `placki.local`
- Dokonaj drugiej konfiguracji *DNS* przekierowując nazwy `gugle.pl` i `www.gugle.pl` na adres strony `google.com`

> Wykorzystaj `nslookup` do testowania nazw *DNS* i poznania adresu ip dla domeny WwW strony firmy Google.


## Wynik

Wykonanie `ping`-u na `placki.local` powinno skomunikować klienta z serwerem.  
Wyszukanie strony `gugle.pl` i `www.gugle.pl` w przeglądarce powinno odtworzyć stronę wyszukiwarki Google.
