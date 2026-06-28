# Portfolio-Studenta
Aplikacja portfolio - React Native / Expo

# Portfolio App — Filip Nocoń

Natywna aplikacja mobilna stworzona w **React Native / Expo** pełniąca funkcję interaktywnego portfolio studenckiego. Aplikacja prezentuje umiejętności, zrealizowane projekty oraz dane kontaktowe autora.

## Widoki aplikacji

### Prototyp Figma — HabitMate (5 ekranów)


 

---<img width="1106" height="471" alt="image" src="https://github.com/user-attachments/assets/9144bfde-7409-4108-96ef-f733b35236a7" />


### Zrzuty ekranu z działającej aplikacji

**Ekran Profilu**
> **Tutaj wstaw screenshot ekranu Profil z działającej aplikacji**

![Profil](Prototyp/screen-profil.png)

---

**Lista Projektów**
> **Tutaj wstaw screenshot ekranu Moje Projekty**

![Projekty](Prototyp/screen-projekty.png)

---

**Szczegóły projektu HabitMate**
> **Tutaj wstaw screenshot ekranu Szczegółów z przyciskiem "Otwórz HabitMate"**

![Szczegóły HabitMate](Prototyp/screen-habitmate.png)

---

**Formularz dodawania projektu**
> **Tutaj wstaw screenshot ekranu Nowy Projekt**

![Nowy Projekt](Prototyp/screen-nowy-projekt.png)

---

**Ekran Kontakt**
> **Tutaj wstaw screenshot ekranu Kontakt**

![Kontakt](Prototyp/screen-kontakt.png)

---

## Opis projektu

Aplikacja portfolio studenta kierunku Informatyka, zaprojektowana zgodnie z wytycznymi Human Interface Guidelines firmy Apple. Umożliwia prezentację umiejętności technicznych, zrealizowanych projektów oraz danych kontaktowych w formie interaktywnej aplikacji mobilnej.

Projekt zawiera również wbudowaną, w pełni działającą aplikację **HabitMate** — tracker nawyków dostępny bezpośrednio z ekranu szczegółów projektu.

---

## Instrukcja uruchomienia

### Wymagania

- Node.js 18+
- npm
- Aplikacja **Expo Go** na telefonie (iOS / Android) — dostępna w App Store i Google Play

### Kroki

```bash
# 1. Sklonuj repozytorium
git clone https://github.com/filipppppppppppp/portfolio-ios.git
cd portfolio-ios

# 2. Zainstaluj zależności
npm install

# 3. Zainstaluj obsługę przeglądarki (opcjonalnie)
npx expo install react-native-web react-dom @expo/metro-runtime

# 4. Uruchom aplikację
npx expo start
```

Po uruchomieniu:
- **Na telefonie** — zeskanuj kod QR aplikacją Expo Go
- **W przeglądarce** — naciśnij klawisz `w` w terminalu

---

## Lista funkcjonalności

| Funkcjonalność | Opis |
|---|---|
| Ekran profilu | Dane studenta, zdjęcie, opis, umiejętności z paskami postępu, edukacja |
| Lista projektów | Karty projektów z kategorią, rokiem, technologiami i statusem |
| Szczegóły projektu | Pełny opis, technologie, link do GitHub, możliwość usunięcia |
| Dodawanie projektów | Formularz z polami: nazwa, opis, technologie, rok, GitHub, kategoria, status, kolor |
| Walidacja formularza | Sprawdzanie wymaganych pól, minimalnej długości, poprawności roku |
| Usuwanie projektów | Usuwanie z potwierdzeniem (Alert) |
| Persystencja danych | Projekty zapisywane lokalnie przez AsyncStorage — nie znikają po restarcie |
| Mini-app HabitMate | Działający tracker nawyków wbudowany w portfolio |
| Odhaczanie nawyków | Zaznaczanie nawyków jako wykonanych z zapisem na dany dzień |
| Statystyki nawyków | Seria, łączna liczba wykonań, skuteczność, wykres 7-dniowy |
| Wyszukiwanie nawyków | Filtrowanie listy nawyków po nazwie i kategorii |
| Ekran kontaktowy | Email i GitHub z możliwością otwarcia lub skopiowania |
| Nawigacja Tab | Bottom Tab Navigator — Profil / Projekty / Kontakt |
| Nawigacja Stack | Stack Navigator wewnątrz zakładki Projekty |

---

## Stos technologiczny

| Warstwa | Technologia |
|---|---|
| Framework | React Native + Expo SDK 51 |
| Nawigacja | React Navigation 6 (Bottom Tabs + Native Stack) |
| Persystencja | AsyncStorage |
| Język | JavaScript (ES2022) |
| Linki systemowe | expo-linking |
| Prototypowanie | Figma |

---

## Struktura projektu

```
portfolio-filip/
├── App.js                              # Punkt wejścia aplikacji
├── app.json                            # Konfiguracja Expo
├── package.json                        # Zależności
├── README.md                           # Dokumentacja
├── Prototyp/                           # Widoki Figma + screenshoty
│   ├── habitmate-figma.png             # Screenshot prototypu z Figmy
│   ├── screen-profil.png               # Screenshot ekranu Profil
│   ├── screen-projekty.png             # Screenshot ekranu Projekty
│   ├── screen-habitmate.png            # Screenshot szczegółów HabitMate
│   ├── screen-nowy-projekt.png         # Screenshot formularza
│   └── screen-kontakt.png             # Screenshot ekranu Kontakt
├── assets/
│   └── avatar.png                      # Zdjęcie profilowe
└── src/
    ├── navigation/
    │   └── AppNavigator.js             # Konfiguracja nawigacji
    ├── screens/
    │   ├── ProfileScreen.js            # Ekran profilu
    │   ├── ProjectsScreen.js           # Lista projektów
    │   ├── ProjectDetailScreen.js      # Szczegóły projektu
    │   ├── AddProjectScreen.js         # Formularz dodawania
    │   └── ContactScreen.js            # Ekran kontaktowy
    ├── habitmate/
    │   ├── HabitMateApp.js             # Nawigator HabitMate
    │   ├── HabitDashboard.js           # Ekran dziś
    │   ├── HabitListScreen.js          # Lista nawyków
    │   ├── HabitDetailScreen.js        # Szczegóły nawyku
    │   ├── AddHabitScreen.js           # Dodaj nawyk
    │   └── habitStorage.js             # AsyncStorage dla nawyków
    ├── storage/
    │   └── storage.js                  # AsyncStorage dla projektów
    └── theme/
        └── colors.js                   # Paleta kolorów (#5B56D0)
```

---

## Kolorystyka

Kolor przewodni: **#5B56D0** (fiolet indygo) — spójny z prototypem HabitMate wykonanym w Figmie.

---

## Autor

**Filip Nocoń**
Przedmiot: Aplikacje mobilne na iOS
Rok akademicki: 2025/2026


