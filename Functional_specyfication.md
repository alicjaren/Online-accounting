# Online-accounting - functional specyfication 
## Internetowy system prowadzenia księgowości - rozliczanie VAT-7 - specyfikacja funkcjonalna

### Funkcje systemu
#### 1. Rejestracja nowego użytkownika
  - Podanie danych użytkownika:
    - imię,
    - nazwisko,
    - adres mailowy,
    - adres zamieszkania,
    - NIP,
    - data urodzenia,
    - numer telefonu,
    - nazwa urzędu skarbowego;
  - Podanie nazwy użytkownika - loginu (system po wprowadzeniu nazwy informuje, czy taki login jest wolny);
  - Utworzenie silnego hasła (system informuje o sile hasła);
 
 
#### 2. Wprowadzenie faktury zakupu do systemu - rejestru nabycia
  - Podanie przez użytkownika:
    - daty wystawienia faktury,
    - numeru faktury,
    - NIP-u sprzedającego,
    - nazwy sprzedającego,
    - przedmiotów zakupu,
    - wartości łącznej brutto,
    - wartości netto dla 23% podatku VAT,
    - wartości podatku naliczonego dla 23% VAT,
    - wartości netto dla 8% podatku VAT,
    - wartości podatku naliczonego dla 8% VAT,
    - wartości netto dla 5% podatku VAT,
    - wartości podatku naliczonego dla 5% VAT,
    - zaznaczenie, czy **podatek naliczony od kolejnych zakupów z faktury podlega odliczeniu**,
    - zaznaczenie, czy kolejne zakupy z wprowadzanej faktury są **środkami trwałymi**;
  - Ustawienie przez system daty wpływu faktry na datę wprowadzenia jej do systemu;
  
    
#### 3. Wprowadzenie faktury sprzedaży do systemu - rejestru sprzedaży
 - Podanie przez użytkownika:
    - daty wystawienia faktury,
    - numeru faktury,
    - NIP-u kupującego,
    - nazwy kupującego,
    - przedmiotów sprzedaży,
    - wartości netto dla 23% podatku VAT,
    - wartości netto dla 8% podatku VAT,
    - wartości netto dla 5% podatku VAT;
 - Wyliczenie i zaksięgowanie przez system kwot podatku należnego dla VAT w wysokościach: 5%, 8% i 23%;
 - Wyliczenie i zaksięgowanie przez system łącznej kwoty brutto sprzedaży;
 
 
#### 4. Dokonanie rozliczenia miesięcznego - uzyskanie danych potrzebnych do wypełnienia deklaracji
  - rozliczenie podatku należnego - wyliczenie przez system dla użytkownika : 
          - ddd
  - rozliczenie podatku naliczonego - wyliczenie przez system dla użytkownika:        
  - podanie przez system kwoty nadwyżki z poprzedniej deklaracji;
  - 
  
  
#### 5. Podgląd ewidencji z każdego miesiąca 
  - podgląd rejestru sprzedaży,
  - podgląd rejestru zakupu;
  - podgląd rozliczenia miesięcznego (kwoty używane w deklaracji składanej w urzędzie skarobowym);
