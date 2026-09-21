# Opis

### setContentView
Funkcja którą tworzysz elementy XML oraz ustawiasz czym jest layout, podstawowo ustawione jest "activity_main".

### Klasa R
Automatycznie generowana klasa która zmienia nazwy XML z katalogu /res w pola w Javie. **NIE EDYTOWAĆ RĘCZNIE.**

### findViewById
Troche jak getElementById w JS, przeszukuje layout i zwraca znaleziony widok. **Musi** być po setContentView bo przed nim layout w javie nie istnieje.

### onCreate
Pierwsza automatycznie wywoływana przez program funkcja w aplikacji mobilnej. Jest wywoływana **tylko raz** przy utworzeniu (otwarciu) aplikacji.

### super.onCreate
Musi być w pierwszej linii, wywołuje wersje z klasy nadrzędnej, w tym przypadku z AppCompatActivity, oraz przygotowuje ekran.

### AndroidManifest.xml
Plik czytany przed otwarciem aplikacji, są w nim zawarte ogólne informacje o aplikacji takie jak:
- Motyw
- Nazwa aplikacji
- Ikona aplikacji
- Uprawnienia aplikacji (do aparatu, lokalizacji itd.)
Jest tu również zadeklarowany każdy poszczególny ekran oraz informacje ogólne o nim np. Czy może on być uruchomiony przez inne aplikacje oraz czy jest on ekranem głównym

### @+id/
Jest to połączenie między XML-em i Javą dzięki niemu możemy odwołać się do elementu XML w Javie.
| Fragment | Znaczenie |
|---|---|
| `@` | Odwołanie się do zasobu |
| `+` | Stwórz nowy zasób, powinno być tylko przy 1 odwołaniu ale nic się nie stanie jak w kolejnych też sie pojawi |
| `id/` | typ zasobu |
| `Nazwa` | Nazwa |


### match_parent
Wartość wysokości lub wysokości, oznacza ona że element zajmie tyle miejsca co element nadrzędny (rodzic).

### dp
**density-independent pixel** - czyli jednostka niezależna od ekranu. System przelicza ją w zależności od ekranu dzięki czemu np. 15dp wygląda tak samo na każdym ekranie.

### sp
**scale-independent pixel** - jednostka niezależna od skali. Używana tylko do tekstu, skaluje rozmiar tekstu w zależności od ustawień skali w telefonie (używają tego np słabowidzący).
