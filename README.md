# 🚗 Czuwak Kierowcy 2.0

**Progresywna aplikacja webowa (PWA) dla kierowców jeżdżących nocą**

Aplikacja przypomina kierowcy o zachowaniu czujności poprzez regularne powiadomienia z systemem alarmowym. Idealana dla długich nocnych tras, szczególnie na autostradach.

## 🎯 Główne funkcje

### 🔔 System przypomnień
- **Konfigurowalne interwały**: 30s, 1min, 2min, 5min, 10min
- **15-sekundowy countdown** z ostrzeżeniem
- **Pełnoekranowy alert** z napisem "CZUWAM!"
- **Timer do następnego przypomnienia**

### 🚨 System alarmowy
- **Automatyczny alarm** po 15 sekundach braku reakcji
- **Własny plik dźwiękowy** (`alarm.mp3`) + syntetyczny backup
- **Intensywne wibracje** (na urządzeniach mobilnych)
- **Migający ekran** jako dodatkowe ostrzeżenie
- **Alarm w pętli** do momentu reakcji kierowcy

### 🛣️ Integracja GPS
- **Automatyczne pauzowanie** gdy pojazd stoi (< 1 km/h)
- **Wznawianie** gdy pojazd ruszy
- **Wyświetlanie prędkości** w czasie rzeczywistym
- **Status pojazdu**: "Jadę" / "Stoję"
- **Dokładność GPS** z informacją o statusie

### 🏎️ Auto-Start (NOWOŚĆ!)
- **Automatyczne włączanie** przy spadku prędkości
- **Konfigurowalna prędkość progowa** (domyślnie 120 km/h)
- **Inteligentna logika**: czeka aż przekroczysz próg, potem monitoruje spadek
- **Idealne na autostradach**: auto-start przy korkach/zwalnianiu

### 📳 System wibracji
- **Wibracje podczas alarmu** z intensywnym wzorem
- **Automatyczne wykrywanie obsługi** dla różnych urządzeń
- **Test wibracji** przy włączeniu opcji
- **Kompatybilność**: Android (pełna), iOS (ograniczona), Desktop (brak)

### 📊 Statystyki i analiza (NOWOŚĆ!)
#### **Zakładka "Statystyki"**:
- **Statystyki sesji**: czas jazdy, liczba alertów, reakcji, skuteczność
- **Średni czas reakcji** z oceną jakości (Doskonały/Dobry/OK/Wolny)
- **Statystyki ogółem**: łączna liczba sesji, całkowity czas, najlepsza seria
- **Możliwość czyszczenia** wszystkich danych

#### **Zakładka "GPS Analytics"**:
- **Analiza prędkości**: aktualna, maksymalna, średnia prędkość
- **Dystans podróży** w kilometrach
- **Analiza typu drogi**: Autostrada/Droga krajowa/Wojewódzka/Miasto
- **Styl jazdy**: Spokojny/Normalny/Dynamiczny/Agresywny
- **Czas w ruchu vs postoje**
- **Historia lokalizacji** z ostatnimi punktami trasy
- **Inteligentne rekomendacje** interwałów na podstawie stylu jazdy

### 📱 Funkcje PWA
- **Wake Lock API** - ekran się nie wygasza
- **Działa offline** po pierwszym załadowaniu
- **Instalowalna** jako aplikacja na telefon
- **Manifest PWA** z ikonami
- **Pełnoekranowy tryb** podczas alarmów

### 🎨 Optymalizacje mobilne
- **Responsywny design** dla wszystkich rozmiarów ekranów
- **Gesture control** - swipe do zamykania alertów
- **Orientacja landscape** z dostosowanym interfejsem
- **Dotykowa optymalizacja** z eliminacją opóźnień
- **Obsługa fold phones** i wąskich ekranów

## 🚀 Jak uruchomić

### Metoda 1: GitHub Pages (online)
1. Wejdź na: `https://lukaszdylka.github.io/czuwak-kierowcy-2-0/`
2. Pozwól na dostęp do lokalizacji i dźwięku
3. Opcjonalnie: "Dodaj do ekranu głównego" (PWA)

### Metoda 2: Lokalnie
1. Pobierz plik `index.html`
2. Otwórz w przeglądarce (Chrome, Firefox, Safari, Edge)
3. Pozwól na uprawnienia GPS i audio

## 🎮 Instrukcja użycia

### Podstawowe uruchamianie:
1. **Wybierz interwał** przypomnień (30s-10min)
2. **Konfiguruj opcje**: auto-start, wibracje
3. **Kliknij "Rozpocznij"** 🟢
4. **Reaguj na przypomnienia** - kliknij/dotknij ekranu w ciągu 15 sekund
5. **Zatrzymaj/Wznów** ⏸️ gdy potrzebujesz przerwy

### Auto-Start na autostradzie:
1. **Zaznacz checkbox** "Auto-start przy spadku prędkości" 
2. **Ustaw próg prędkości** (np. 120 km/h dla autostrady)
3. **Jedź normalnie** - gdy prędkość spadnie, czuwak włączy się automatycznie
4. **Przykład**: 150 km/h → 110 km/h = auto-start!

### Zakładki nawigacyjne:
- **"Główne"** - podstawowe sterowanie aplikacją
- **"Statystyki"** - analiza wydajności i czasu reakcji
- **"GPS Analytics"** - szczegółowa analiza jazdy i rekomendacje

## 🔧 Wymagania techniczne

### Przeglądarka:
- **Chrome** 60+ (zalecane - pełna obsługa)
- **Firefox** 55+ (dobra obsługa)
- **Safari** 13+ (ograniczone wibracje)
- **Edge** 79+ (dobra obsługa)

### Uprawnienia:
- ✅ **Lokalizacja** - do odczytu prędkości GPS
- ✅ **Audio** - do odtwarzania alarmu
- ✅ **Wake Lock** - zapobieganie wygaszeniu ekranu
- ✅ **Wibracje** - powiadomienia haptyczne (opcjonalne)

### Opcjonalne pliki:
- `alarm.mp3` - własny dźwięk alarmu (formaty: MP3, WAV, OGG)

## ⚠️ Bezpieczeństwo - WAŻNE!

### 🛡️ Zasady bezpiecznego użytkowania:
- **Testuj przed jazdą** - sprawdź wszystkie funkcje w bezpiecznym miejscu
- **To dodatek, nie zamiennik** - czuwak wspomaga, ale nie zastępuje czujności
- **Mocuj telefon** - zabezpiecz urządzenie w samochodzie
- **Dostosuj do warunków** - używaj rekomendacji z GPS Analytics
- **Nie polegaj tylko na aplikacji** - zachowaj zdrowy rozsądek

### 🚫 Kiedy NIE używać:
- W trudnych warunkach pogodowych
- Na nieznanej drodze wymagającej uwagi
- Gdy czujesz się bardzo zmęczony (lepiej odpocząć!)
- W gęstym ruchu miejskim

## 🔊 Konfiguracja dźwięku

### Dodanie własnego alarmu:
1. **Nagraj/znajdź** plik dźwiękowy (2-5 sekund)
2. **Nazwij** `alarm.mp3` 
3. **Umieść** w tym samym folderze co `index.html`
4. **Sprawdź** w konsoli przeglądarki czy się załadował

### Zalecane parametry:
- **Format**: MP3, 128-320 kbps
- **Długość**: 2-5 sekund (odtwarza się w pętli)
- **Typu**: alarm samochodowy, syrena, klakson, dzwonek

## 📊 Statusy aplikacji

| Status | Znaczenie |
|--------|-----------|
| `Nieaktywny` | Aplikacja wyłączona |
| `Gotowy do auto-startu` | Auto-start włączony, oczekuje |
| `Gotowy - Prędkość: XXX km/h` | Prędkość powyżej progu |
| `🚀 AUTO-START!` | Wykryto spadek prędkości |
| `Aktywny - Monitorowanie` | Czuwak działa normalnie |
| `Wstrzymany - Pojazd stoi` | Auto-pauza przy prędkości < 1 km/h |
| `🚨 ALARM!` | Brak reakcji na przypomnienie |

## 📈 Funkcje analityczne

### Typy dróg (auto-wykrywanie):
- **Autostrada**: >100 km/h średnia, >80 km/h maksymalna
- **Droga krajowa**: >80 km/h maksymalna, >50 km/h średnia
- **Droga wojewódzka**: >50 km/h maksymalna, >30 km/h średnia
- **Miasto**: prędkości miejskie
- **Postój**: brak ruchu

### Style jazdy:
- **Spokojny**: minimalne zmiany prędkości
- **Normalny**: standardowe przyspieszenia/hamowania
- **Dynamiczny**: częste zmiany prędkości
- **Agresywny**: bardzo częste, gwałtowne zmiany

### Rekomendacje interwałów:
- **Autostrada + spokojny styl**: 2-5 minut
- **Miasto + agresywny styl**: 30s-1 minuta
- **Drogi krajowe**: 1-2 minuty
- **Dynamika jazdy**: dostosowanie automatyczne

## 🛠️ Rozwój projektu

### Technologie:
- **HTML5** - struktura z semantycznymi znacznikami
- **CSS3** - responsywny design z animacjami
- **Vanilla JavaScript** - logika aplikacji (ES6+)
- **Geolocation API** - GPS i analiza ruchu
- **Web Audio API** - syntetyczny dźwięk backup
- **Vibration API** - wibracje mobilne
- **Wake Lock API** - zapobieganie uśpieniu
- **Service Worker** - cache offline i PWA

### Zgłaszanie błędów:
Jeśli znajdziesz błąd lub masz pomysł na ulepszenie, stwórz **Issue** w repozytorium GitHub.

## 📄 Licencja

**MIT License** - możesz swobodnie używać, modyfikować i dystrybuować.

## 🤝 Współtworzenie

1. **Fork** repozytorium
2. **Stwórz** branch z funkcją (`git checkout -b nowa-funkcja`)
3. **Commit** zmiany (`git commit -m 'Dodaj nową funkcję'`)
4. **Push** do branch (`git push origin nowa-funkcja`)
5. **Stwórz** Pull Request

---

## 🎉 Changelog

### v2.0 (aktualna)
- ✨ **Auto-Start** przy spadku prędkości
- 📊 **System statystyk** z trzema zakładkami nawigacyjnymi
- 🗺️ **GPS Analytics** - analiza typu drogi, stylu jazdy, rekomendacje
- 📳 **Wibracje** z obsługą różnych platform
- 🔊 **Obsługa własnych plików audio** (`alarm.mp3`)
- 🎨 **Przeprojektowany UI** - responsywny design, lepsze animacje
- 📱 **Pełna optymalizacja PWA** - offline, instalowalna
- 🛣️ **Inteligentne zarządzanie sesją** na podstawie GPS
- 🎯 **Gesture control** - swipe do zamykania alertów
- 🔄 **Smart Wake Lock** - automatyczne zarządzanie ekranem

### v1.0
- 🔔 Podstawowy system przypomnień
- 🚨 Alarm dźwiękowy i wizualny
- 📍 Podstawowa integracja GPS
- 📱 Obsługa PWA
- 🌙 Ciemny motyw

---

**Bezpiecznej jazdy!** 🚗💨

*Pamiętaj: żadna aplikacja nie zastąpi odpowiedniego wypoczynku przed podróżą!*

## 💡 Tips & Tricks

### Dla kierowców zawodowych:
- Używaj **GPS Analytics** do optymalizacji przerw
- **Statystyki reakcji** pomagają monitorować zmęczenie
- **Auto-start** idealny na długich trasach autostradowych

### Dla kierowców okazjonalnych:
- Zacznij od **1-2 minut** interwału
- Włącz **wibracje** na telefonie
- Sprawdź **rekomendacje** po każdej trasie

### Optymalizacja baterii:
- Aplikacja używa **Wake Lock** oszczędnie
- **GPS** włącza się tylko podczas aktywnej sesji
- **Offline PWA** redukuje zużycie danych
