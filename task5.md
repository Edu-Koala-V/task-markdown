# Zarządzanie usługami i Harmonogramem zadań w Windows 11
## Wymagania wstępne
- Maszyna wirtualna z systemem **Windows 11**.
## Treść zadania
- Uruchom przystawkę "**Usługi**" (_services.msc_).
- Zmień tryb uruchamiania usługi "**Klient DNS**" (_Dnscache_) na **ręczny**. Upewnij się, że usługa nie jest uruchomiona.
- Sprawdź, czy usługa "**Windows Update**" (_wuauserv_) jest w trybie **automatycznym (opóźniony start)**. Jeśli nie, zmień jej tryb na ten wskazany.
- Uruchom przystawkę "**Harmonogram zadań**" (_taskschd.msc_).
- Utwórz nowe, **podstawowe zadanie** o nazwie "**`Sprawdź DNS`**", które będzie uruchamiane **raz dziennie**.
- Zadanie powinno wywoływać program `ipconfig.exe` z argumentem `/flushdns`.
- Upewnij się, że zadanie jest skonfigurowane do uruchamiania nawet, jeśli komputer nie był włączony o wyznaczonej porze (opcja "Uruchom szybko zadanie, jeśli pominięto zaplanowane uruchamianie").
- Uruchom zadanie ręcznie i zweryfikuj w CMD, czy pamięć podręczna DNS została wyczyszczona.
