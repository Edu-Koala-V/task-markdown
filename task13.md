# Domena AD użytkownicy, profile i czas

## Wymagania wstępne

- Maszyna virtualna z systemem _**Windows Server 2025**_.
- Maszyna virtualna z systemem _**Windows 11 Pro**_.
- Maszyna virtualna z systemem _**Windows 11 Pro**_.

Zmień nazwy maszyn na Serv, Host1 i Host2.  

Tylko maszyna z **Serwerem** powinna mieć po dwie karty sieciowe (`NAT` i `sieć wewnętrzna`).  
Dla klientów pozostaw jedynie jedną, działającą w trybie `sieć wewnętrzna`.

## Treść zadania

- Skonfiguruj domenę Active Directory o nazwie _`klubowicze.local`_.
- Utwórz dwóch użytkowników i określ ich czasy logowania do domeny:

| Login        |   Nazwa    |      Hasło | Dozwolony zakres czasu na logowanie |
| :----------- | :--------: | ---------: | ----------------------------------: |
| _klubowicz1_ |  **Adam**  | `ZAQ!2wsx` |                 `08:00` _-_ `16:00` |
| _klubowicz2_ | **Teresa** | `XSW@1qaz` |                 `16:00` _-_ `22:00` |

- Przygotuj profile mobilne dla obu użytkowników.
- Dodaj użytkownika o nazwie **Nadzorca** bez ograniczeń czasowych ale z profilem mobilnym

## Wynik

- W zależności od bieżącej godziny dostępne jest logowanie jedynie dla dwóch z trzech nowych użytkowników.  

- Po zalogowaniu się na `Host1` i zmianie tła pulpitu, ustawienie to zostanie automatycznie przeniesione na drugiego klienta domeny, gdy zalogujesz się tym samym kontem na `Host2`.
