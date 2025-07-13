# 🚗 Czuwak Kierowcy 2.0

**Progresywna aplikacja webowa (PWA) dla kierowców jeżdżących nocą**

Aplikacja przypomina kierowcy o zachowaniu czujności poprzez regularne powiadomienia z systemem alarmowym. Idealana dla długich nocnych tras, szczególnie na autostradach.

## 🎯 Główne funkcje

### 🔔 System przypomnień
- **Konfigurowalne interwały**: 30s, 1min, 2min, 5min, 10min
- **Duży czerwony przycisk** z napisem "CZUWAM!" 
- **15-sekundowy countdown** z ostrzeżeniem
- **Timer do następnego przypomnienia**

### 🚨 System alarmowy
- **Automatyczny alarm** po 15 sekundach braku reakcji
- **Własny plik dźwiękowy** (`alarm.mp3`) + syntetyczny backup
- **Migający ekran** jako dodatkowe ostrzeżenie
- **Alarm w pętli** do momentu reakcji kierowcy

### 🛣️ Integracja GPS
- **Automatyczne pauzowanie** gdy pojazd stoi (< 1 km/h)
- **Wznawianie** gdy pojazd ruszy
- **Wyświetlanie prędkości** w czasie rzeczywistym
- **Status pojazdu**: "Jadę" / "Stoję"

### 🏎️ Auto-Start (NOWOŚĆ!)
- **Automatyczne włączanie** przy spadku prędkości
- **Konfigurowalna prędkość progowa** (domyślnie 120 km/h)
- **Inteligentna logika**: czeka aż przekroczysz próg, potem monitoruje spadek
- **Idealne na autostradach**: auto-start przy korkach/zwalnianiu

### 📱 Funkcje PWA
- **Wake Lock API** - ekran się nie wygasza
- **Działa offline** po pierwszym załadowaniu
- **Instalowalna** jako aplikacja na telefon
- **Manifest PWA** z ikonami

## 🚀 Jak uruchomić

### Metoda 1: GitHub Pages (online)
1. Wejdź na: `https://twoja-nazwa.github.io/czuwak-kierowcy-2-0`
2. Pozwól na dostęp do lokalizacji i dźwięku
3. Opcjonalnie: "Dodaj do ekranu głównego" (PWA)

### Metoda 2: Lokalnie
1. Pobierz plik `czuwak-kierowcy-2.0.html`
2. Otwórz w przeglądarce (Chrome, Firefox, Safari, Edge)
3. Pozwól na uprawnienia GPS i audio

## 🎮 Instrukcja użycia

### Podstawowe uruchamianie:
1. **Wybierz interwał** przypomnień (1-10 minut)
2. **Kliknij "Rozpocznij"** 🟢
3. **Reaguj na przypomnienia** - kliknij czerwony przycisk w ciągu 15 sekund
4. **Zatrzymaj/Wznów** ⏸️ gdy potrzebujesz przerwy

### Auto-Start na autostradzie:
1. **Zaznacz checkbox** "Auto-start przy spadku prędkości" 
2. **Ustaw próg prędkości** (np. 120 km/h dla autostrady)
3. **Jedź normalnie** - gdy prędkość spadnie, czuwak włączy się automatycznie
4. **Przykład**: 150 km/h → 110 km/h = auto-start!

## 🔧 Wymagania techniczne

### Przeglądarka:
- **Chrome** 60+ (zalecane)
- **Firefox** 55+
- **Safari** 13+
- **Edge** 79+

### Uprawnienia:
- ✅ **Lokalizacja** - do odczytu prędkości GPS
- ✅ **Audio** - do odtwarzania alarmu
- ✅ **Wake Lock** - zapobieganie wygaszeniu ekranu

### Opcjonalne pliki:
- `alarm.mp3` - własny dźwięk alarmu (formaty: MP3, WAV, OGG)
- `manifest.json` - manifest PWA
- `icon-192.png`, `icon-512.png` - ikony aplikacji

## ⚠️ Bezpieczeństwo - WAŻNE!

### 🛡️ Zasady bezpiecznego użytkowania:
- **Testuj przed jazdą** - sprawdź wszystkie funkcje w bezpiecznym miejscu
- **To dodatek, nie zamiennik** - czuwak wspomaga, ale nie zastępuje czujności
- **Mocuj telefon** - zabezpiecz urządzenie w samochodzie
- **Dostosuj do warunków** - zmień interwały zależnie od sytuacji
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

## 🛠️ Rozwój projektu

### Technologie:
- **HTML5** - struktura
- **CSS3** - style z animacjami
- **Vanilla JavaScript** - logika aplikacji
- **Geolocation API** - GPS
- **Web Audio API** - syntetyczny dźwięk
- **Wake Lock API** - zapobieganie uśpieniu
- **Service Worker** - cache offline

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
- 🔊 **Obsługa własnych plików audio** (`alarm.mp3`)
- 🎨 **Ulepszone UI** - większy przycisk, lepsze animacje
- 📱 **Optymalizacja PWA** - lepsza instalowalność
- 🛣️ **Inteligentne pauzowanie** na podstawie GPS

### v1.0
- 🔔 Podstawowy system przypomnień
- 🚨 Alarm dźwiękowy i wizualny
- 📍 Integracja GPS
- 📱 Obsługa PWA
- 🌙 Ciemny motyw

---

**Bezpiecznej jazdy!** 🚗💨

*Pamiętaj: żadna aplikacja nie zastąpi odpowiedniego wypoczynku przed podróżą!*
