# Zarządzanie udziałami sieciowymi i uprawnieniami w Windows 11 (fsmgmt.msc)
## Wymagania wstępne
- Maszyna wirtualna z systemem **Windows 11**.
- Utwórz dwóch użytkowników: **`Manager`** (z grupy "Administratorzy") i **`Pracownik`** (z grupy "Użytkownicy").
- Utwórz na dysku C: (lub innym) folder o nazwie **`DaneFirmowe`**.
## Treść zadania
- Uruchom przystawkę "**Foldery udostępnione**" (_fsmgmt.msc_).
- Utwórz nowy udział sieciowy dla folderu **`C:\DaneFirmowe`** o nazwie "**`Firmowe`**".
- Skonfiguruj **uprawnienia udziału** w następujący sposób:
    - Grupa **`Administratorzy`** ma mieć **pełną kontrolę (FULL)**.
    - Użytkownik **`Manager`** ma mieć **pełną kontrolę (FULL)**.
    - Użytkownik **`Pracownik`** ma mieć **tylko odczyt (READ)**.
    - Upewnij się, że grupa **"Wszyscy" nie ma dostępu** do udziału.
- **Zweryfikuj dostęp** do udziału z poziomu innej maszyny wirtualnej (jeśli dostępna) lub z konta **`Pracownik`** i **`Manager`** na tej samej maszynie. Spróbuj utworzyć/modyfikować pliki jako `Pracownik` i `Manager`.
- Przejdź do właściwości folderu `C:\DaneFirmowe` w Eksploratorze plików (Prawy przycisk myszy > Właściwości > Zabezpieczenia). **Opisz, w jaki sposób uprawnienia NTFS mogą nadpisać (ograniczyć) uprawnienia udostępniania**.
