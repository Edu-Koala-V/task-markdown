# Windows IIS - strona www

## Wymagania wstępne

- Maszyna virtualna z systemem _**Windows Server 2025**_.
- Maszyna virtualna z systemem _**Ubuntu 24.04 Desktop**_.
- Maszyna virtualna z systemem _**Windows 11 Pro**_.

Każda maszyna powinna mieć po dwie karty sieciowe (`NAT` i `sieć wewnętrzna`).

## Treść zadania


- Skonfiguruj *DNS* na nazwę www.koala.local przekierowujący na adres serwera.
- Zmodyfikuj domyślną stronę w menedzerze IIS aby wskazywała na nowy plik `index.html`.
- Utwórz w odpowiedniej, czyli domyślnej lokalizacji plików strony IIS nowy plik `index.html`.

Zawartość pliku `index.html`

```html
Strona <b>działa</b> <i>poprawnie</i>.
```

## Wynik

Pokarz na obu klientach że po wpisaniu w przeglądarce adresu `www.koala.local` uruchomi się strona o następującej treści:

---

Strona <b>działa</b> <i>poprawnie</i>.

---
