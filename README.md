oitestool
=========

### Skrypt napisany w Bashu do testowania zadań z Olimpiady Informatycznej.

Dla każdego testu skrypt wyświetli:

- nazwę testu
- czas działania
- zajętą pamięć *(UWAGA: podany rezultat może różnić się od rzeczywistego)*
- czy odpowiedź jest zaliczona (i ewentualny powód niezaliczenia)

Pod zakończeniu działania zostanie wyświetlone podsumowanie:

- ilość dobrych odpowiedzi
- ilość niezaliczonych odpowiedzi (z podziałem na powody niezaliczenia)
- maksymalna pamięć wykorzystana podczas testowania
- maksymalny czas działania na pojedynczym teście
- sumaryczny czas wykonywania obliczeń

### Opcje
Aktualne możliwości skryptu:

- testowanie nieskompilowanego programu - zostanie on skompilowany:
  - według pliku *Makefile* - jeśli istnieje
  - z flagami według ustaleń Olimpiady: *-Wall -O2 -static -std=gnu++0x*
- testowanie skompilowanego programu
- możliwość podania programu, który sam sprawdzi, czy odpowiedź jest poprawna
- możliwość wskazania folderu z plikami wejściowymi (domyślnie: folder aktualny)
- możliwość wskazania folderu z odpowiedziami (domyślnie: ten sam, co z plikami wejściowymi)
- podanie nazw konkretnych testów zamiast całego folderu z testami (działają również regexpy)
- możliwość generowania odpowiedzi
- ustalenie limitu czasowego
- ustalenie limitu pamięci
- możliwość zapisania nazw niezaliczonych testów do pliku
- wyświetlenie pomocy zawierącej opis opcji

### Wymagania
System operacyjny: 

- Linux

Skrypt wykorzystuje do działania programy:

- awk
- sed
- time

Opcjonalnie - do ustawienia limitu czasowego:

- timeout
