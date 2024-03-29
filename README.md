# OptimumLap Simulator
## Opis
Program do symulacji punktów ustawień samochodu, stworzony w celu wspomagania pracy grupy zajmującej się aerodynamiką. Grupa dostarcza dane w postaci wartości Cl (siła nośna) oraz Cd (opór aerodynamiczny), a następnie program wykonuje symulacje dla wszystkich zaznaczonych torów. Wyniki symulacji są eksportowane do pliku CSV.

## Proces
1. Dostarczenie danych przez grupę aerodynamiczną:
Grupa zajmująca się aerodynamiką dostarcza dane dotyczące siły nośnej (Cl) oraz oporu aerodynamicznego (Cd) dla różnych ustawień samochodu.

2. Symulacje torów:
Program OptimumLap wykonuje symulacje dla wszystkich zaznaczonych torów, wykorzystując dostarczone dane Cl i Cd. Wyniki symulacji są eksportowane do plików CSV.

3. Porównanie konfiguracji:
* Program w języku Python wczytuje dane z plików CSV, grupuje wyniki dla poszczególnych ustawień samochodu i przeprowadza symulację zawodów "między ustawieniami". Punkty są przyznawane za każdy event, a następnie program wypisuje punkty przyznane każdej konfiguracji w celu porównawczym oraz wyboru najlepszej z możliwych, dającej maksymalną lokalną ilość punktów.
* Program w języku python wczytuje dane z plików CSV oraz wyników konkretnych zawodów. Program realizuje założenia podane punkt wyżej, lecz do porównania używa wyników ubiegłorocznych zawodów.

4. Dodatkowe funkcje:
Program może wyświetlać uporządkowane dokładne dane dotyczące każdego ustawienia, takie jak: czas, punkty, miejsce w danej konkurencji.


![Diagram działania programu](https://github.com/Fileq03/aero/blob/main/diagram.drawio.pdf)

## Instrukcje użycia
Uruchom program i dostarcz dane aerodynamiczne.
Zaznacz tory, na których chcesz przeprowadzić symulacje.
Program automatycznie eksportuje wyniki do plików CSV.
Uruchom skrypt Pythona do analizy wyników, porównywania ustawień i przyznawania punktów.
Symulacja "między ustawieniami"
```python
python simulate_race.py
```
Porównanie z realnymi zawodami
```python
python compare_to_real_races.py
```
Autorzy
Filip Michalski
