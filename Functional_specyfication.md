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
  - Wprowadzenie przez system faktury do rozliczenia, pod warunkiem, że od daty wystawienia do daty wprowadzenia upłynęły maksymalnie 3 miesiące, w przeciwnym razie system informuje o braku możliwości odliczenia podatku VAT z tej faktury;
  
    
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
  - rozliczenie podatku należnego - wyliczenie przez system dla użytkownika: 
    - podstawy opodatkowania oraz podatku należnego dla towarów i usług opodatkowanych stawką 5%,
    - podstawy opodatkowania oraz podatku należnego dla towarów i usług opodatkowanych stawką 8%,
    - podstawy opodatkowania oraz podatku należnego dla towarów i usług opodatkowanych stawką 23%,
    - sumy podstaw opodatkowania oraz sumy podatku należnego;
  - rozliczenie podatku naliczonego - wyliczenie przez system dla użytkownika:
    - wartości netto nabycia towarów i usług zaliczanych do środków trwałych,
    - wartości podatku naliczonego z nabytych towarów i usług zaliczanych do środków trwałych,
    - wartości netto nabycia towrów i usuług pozostałych,
    - wartości podatku naliczonrgo z nabytych towarów i usług pozostałych;
  - podanie przez system kwoty nadwyżki z poprzedniej deklaracji (przy pierwszym skorzystaniu z usługi system poprosi użytkownika o podanie tej kwoty);
  - podanie przez system łącznej kwoty podatku naliczonego do odliczenia;
  - podanie przez system kwoty podatku podlegającego wpłacie do urzędu skarbowego;
  - podanie przez system kwoty nadwyżki podatku naliczonego nad należnym (jest ona równa 0, gdy kwota podatku podlegającego wpłacie do urzędu skarbowego jest większa od 0);
  - jeśli występuje nadwyżka podatku naliczonego nad należnym, wprowadzenie przez użytkownika: 
      - łącznej kwoty do zwrotu na rachunek bankowy,
      - kwoty do zwrotu w terminie 25 dni,
      - kwoty do zwrotu w terminie 60 dni,
      - kwoty do zwrotu w terminie 180 dni.
  - podanie przez system kwoty do przeniesienia na następny okres rozliczeniowy.
  
  
#### 5. Podgląd ewidencji z każdego miesiąca 
  - podgląd rejestru sprzedaży,
  - podgląd rejestru zakupu,
  - podgląd rozliczenia miesięcznego (kwoty używane w deklaracji składanej w urzędzie skarobowym);
  
  
#### 6. Pobranie pliku w formacie PDF dla każdego miesiąca
  - rejestr sprzedaży,
  - rejestr zakupu,
  - rozliczenie miesięczne (kwoty używane w deklaracji składanej w urzędzie skarobowym);
 
 
#### 7. Przypomnienie drogą mailową o konieczności dokonania rozliczenia miesięcznego i złożenia deklaracji 20. dnia każdego miesiąca



### Uwagi formalne
  1. Obowiązującym w systemie słownikiem stawek VAT są stawki: 5%, 8% i 23%;
  2. Jednostką dla wszystkich kwot jest Złoty polski (PLN);
  3. Kwoty występujące w rejestrze sprzedaży i zakupu są podawane z dokładnością do 2 miejsc po przecinku;
  4. Wymaganą dokładnością kwoty podczas wprowadzania faktur do rejestrów są 2 miejsca po przecinku;
  5. Wszystkie kwoty dla dokonania rozliczenia do urzędu skarbowego podawane są z zaokrągleniem do pełnych złotych;
  6. Wszystkie kwoty dla dokonania rozliczenia do urzędu skarbowego, które podaje użytkowik muszą być podawane z zaokrągleniem do pełnych złotych.
  
  
  
  ### Sposób korzystania z systemu
    1. Użytkownik odwiedza stronę serwisu;
    2. Użytkownik rejestruje się w serwsie, gdy chce rozpocząć korzystanie z usługi;
    3. Użytkownik loguje się przy użyciu loginu oraz hasła, jeśli wcześniej zarejestrował się w serwisie;
    
