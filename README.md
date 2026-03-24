<p align="center">
  <img src="https://visitor-badge.laobi.icu/badge?page_id=Fattcat.Diy-FPV-Drone" alt="Visitors"/>

# 🚁 DIY FPV Long Range Dron – Kompletný návod

> **7" Long Range FPV Dron** | 5km dosah | 200g nosnosť | GPS RTH | LED ovládanie | Tlačený rám (PETG-CF)

---

## 📋 Obsah

- [Prehľad projektu](#-prehľad-projektu)
- [Nákupný zoznam](#-nákupný-zoznam)
- [Potrebné náradie](#-potrebné-náradie)
- [Schéma zapojenia](#-schéma-zapojenia)
- [Tlač rámu](#️-tlač-rámu)
- [Mechanická zostava](#-mechanická-zostava)
- [Elektrické zapojenie](#-elektrické-zapojenie)
- [Konfigurácia softvéru](#-konfigurácia-softvéru)
- [Nastavenie ovládača EdgeTX](#-nastavenie-ovládača-edgetx)
- [Konfigurácia iNav](#-konfigurácia-inav)
- [Nastavenie LED](#-nastavenie-led)
- [Testovanie](#-testovanie)
- [Hmotnostný rozpočet](#️-hmotnostný-rozpočet)
- [Legislatíva SR](#️-legislatíva-sr)
- [Troubleshooting](#-troubleshooting)

---

## 🎯 Prehľad projektu

| Parameter | Hodnota |
|---|---|
| Rám | 7" (tlačený PETG-CF) |
| Dosah RC linku | 5–15 km (ELRS 900MHz) |
| Nosnosť | 200g payload |
| Čas letu | ~17 min (6S 4000mAh) |
| Video systém | DJI O3 Air Unit (digital HD) |
| Autopilot | iNav (GPS, RTH, Waypoints) |
| Celková váha | ~1285g (s batériou + payloadom) |
| Kategória EÚ | C2 (preukaz A2) |
| Odhadovaná cena | ~700–900 € |

---

## 🛒 Nákupný zoznam

### 🏗️ Rám a mechanika

| # | Komponent | Špecifikácia | Počet | Cena (€) | Kde kúpiť |
|---|---|---|---|---|---|
| 1 | Rám 7" (alebo tlač) | TBS Source One 7" / tlačený PETG-CF | 1 | 0–45 € | Printables / Banggood |
| 2 | Motory | 2507, 1700KV, 6S | 4 | 25 €/ks | AliExpress / GetFPV |
| 3 | Vrtule 7" | HQProp 7x4x3 bi-blade | 2 sady | 8 € | AliExpress |
| 4 | Skrutky M3 | Rôzne dĺžky (6mm, 10mm, 16mm) | 1 sada | 5 € | AliExpress |
| 5 | Heat inserts M3 | Mosadzné, 4mm dĺžka | 20 ks | 3 € | AliExpress |
| 6 | Vibration dampener | M3 gumové | 4 ks | 3 € | AliExpress |

### ⚡ Elektronika – Flight Stack

| # | Komponent | Špecifikácia | Počet | Cena (€) | Kde kúpiť |
|---|---|---|---|---|---|
| 7 | FC + ESC Stack | SpeedyBee F405 V4 + 55A 4in1 | 1 | 85 € | SpeedyBee / AliExpress |
| 8 | GPS modul | Beitian BN-880 (u-blox M8N + kompas) | 1 | 18 € | AliExpress |
| 9 | Capacitor 1000µF 35V | Low ESR, na ESC | 1 | 2 € | AliExpress |
| 10 | XT60 konektor (samec) | Pre batériu | 2 ks | 2 € | AliExpress |

### 📡 RC Link

| # | Komponent | Špecifikácia | Počet | Cena (€) | Kde kúpiť |
|---|---|---|---|---|---|
| 11 | Ovládač (Radio) | RadioMaster Boxer (EdgeTX) | 1 | 110 € | RadioMaster |
| 12 | TX modul ELRS | NamimnoRC Voyager 900MHz | 1 | 30 € | AliExpress |
| 13 | RX prijímač ELRS | BetaFPV Nano 900MHz | 1 | 15 € | AliExpress |
| 14 | Anténa 900MHz (dron) | Dipól T-anténa | 1 | 5 € | AliExpress |

### 📹 FPV Video Systém

| # | Komponent | Špecifikácia | Počet | Cena (€) | Kde kúpiť |
|---|---|---|---|---|---|
| 15 | FPV kamera + VTX | DJI O3 Air Unit | 1 | 180 € | DJI / AliExpress |
| 16 | FPV okuliare | DJI Goggles Integra (alebo použité G2) | 1 | 350 € | DJI |
| 17 | Anténa DJI | Stock anténa (v balení) | – | 0 € | – |

### 💡 LED systém

| # | Komponent | Špecifikácia | Počet | Cena (€) | Kde kúpiť |
|---|---|---|---|---|---|
| 18 | WS2812B LED | Individuálne LED, 5V | 2 ks | 2 € | AliExpress |
| 19 | Kábel 3-žilový | 26AWG, 30cm | 1 | 1 € | AliExpress |

### 🔋 Napájanie

| # | Komponent | Špecifikácia | Počet | Cena (€) | Kde kúpiť |
|---|---|---|---|---|---|
| 20 | Batéria LiPo | CNHL 6S 4000mAh 100C | 2 ks | 42 €/ks | CNHL / AliExpress |
| 21 | Nabíjačka | HOTA D6 Pro (duálna) | 1 | 55 € | AliExpress |
| 22 | Paralelný kábel XT60 | 2S paralelný nabíjací kábel | 1 | 5 € | AliExpress |
| 23 | LiPo bezpečnostný vak | Na skladovanie | 1 | 8 € | AliExpress |

### 🖨️ Tlač rámu – materiál

| # | Komponent | Špecifikácia | Počet | Cena (€) | Kde kúpiť |
|---|---|---|---|---|---|
| 24 | Filament PETG-CF | Bambu Lab PETG-CF 500g | 1 | 28 € | bambulab.com |
| 25 | Tryska Hardened Steel | 0.4mm, pre Bambu A1 | 1 | 8 € | bambulab.com |

### 💰 Celkové náklady

| Kategória | Cena |
|---|---|
| Mechanika + rám | ~66 € |
| Elektronika (FC, GPS) | ~107 € |
| RC Link | ~160 € |
| Video systém | ~530 € |
| LED | ~3 € |
| Batérie + nabíjanie | ~110 € |
| Tlač (filament + tryska) | ~36 € |
| **CELKOM** | **~1012 €** |

> 💡 **Tip:** Bez DJI okularov (použité ~200€) a s Walksnail Avatar (~120€) namiesto O3 sa zmestíš pod 700€

---

## 🔧 Potrebné náradie

| Náradie | Použitie | Cena |
|---|---|---|
| Spájkovačka (min. 60W) | Spájkovanie všetkých spojov | 20–50 € |
| Cín (60/40 alebo 63/37) | – | 5 € |
| Multimeter | Meranie napätia, kontinuity | 10–20 € |
| Kliešte na drôty | Krátenie káblov | 8 € |
| Skrutkovač sada (M2, M3) | Montáž | 10 € |
| Teplovzdušná pištoľ / spájkovačka | Vtlačenie heat inserts | (spájkovačka stačí) |
| Zmršťovacie bužírky | Izolácia spojov | 3 € |
| Kapton páska | Izolácia FC, ESC | 2 € |
| Loctite Blue 243 | Zaistenie skrutiek | 5 € |
| Bambu Lab A1 3D tlačiareň | Tlač rámu | (vlastná) |
| PC / Laptop | Konfigurácia softvéru | (vlastný) |

---

## 📐 Schéma zapojenia

```
                        ┌─────────────────────────────────────┐
                        │           BATÉRIA 6S LiPo           │
                        │           XT60 konektor             │
                        └──────────────┬──────────────────────┘
                                       │ (+) a (-)
                        ┌──────────────▼──────────────────────┐
                        │         4-in-1 ESC (55A)            │
                        │  ┌────┐ ┌────┐ ┌────┐ ┌────┐       │
                        │  │M1  │ │M2  │ │M3  │ │M4  │       │
                        │  └──┬─┘ └──┬─┘ └──┬─┘ └──┬─┘       │
                        │     │      │      │      │          │
                        │  Motor  Motor  Motor  Motor         │
                        │  (3 drôty na každý motor)           │
                        │                                     │
                        │  5V BEC out ──────────────────────► │
                        └──────────────┬──────────────────────┘
                                       │ (stack konektor)
                        ┌──────────────▼──────────────────────┐
                        │      FLIGHT CONTROLLER (FC)         │
                        │       SpeedyBee F405 V4             │
                        │                                     │
                        │  UART1 ──────────────────► GPS      │
                        │  UART2 ──────────────────► ELRS RX  │
                        │  UART3 ──────────────────► DJI O3   │
                        │  LED_STRIP pin ──────────► WS2812B  │
                        │  5V out ─────────────────► WS2812B  │
                        │  GND ────────────────────► WS2812B  │
                        └─────────────────────────────────────┘

MOTORY – smer otáčania (props in konfigurácia):
        M2 (CCW) ──── M1 (CW)
            │    RÁM    │
        M3 (CW)  ──── M4 (CCW)

GPS MODUL (BN-880):
    FC UART1 TX ──► GPS RX
    FC UART1 RX ──► GPS TX
    FC I2C SDA  ──► Kompas SDA
    FC I2C SCL  ──► Kompas SCL
    FC 5V       ──► GPS VCC
    FC GND      ──► GPS GND

ELRS PRIJÍMAČ (900MHz Nano):
    FC UART2 TX ──► RX UART RX
    FC UART2 RX ──► RX UART TX
    FC 5V       ──► RX VCC
    FC GND      ──► RX GND

DJI O3 AIR UNIT:
    FC UART3 TX ──► O3 RX
    FC UART3 RX ──► O3 TX
    FC 9V/12V   ──► O3 VIN (z ESC)
    FC GND      ──► O3 GND

WS2812B LED (2 kusy v sérii):
    FC LED_STRIP ──► LED1 DIN
    LED1 DOUT    ──► LED2 DIN
    FC 5V        ──► LED1 VCC + LED2 VCC
    FC GND       ──► LED1 GND + LED2 GND
```

---

## 🖨️ Tlač rámu

### Nastavenia pre Bambu Lab A1 – PETG-CF

| Parameter | Hodnota |
|---|---|
| Tryska | **Hardened Steel 0.4mm** (POVINNÁ!) |
| Teplota trysky | 240–250°C |
| Teplota podložky | 70–80°C |
| Výplň (Infill) | **50% Gyroid** |
| Počet stien (Walls) | **5 perimetrov** |
| Rýchlosť tlače | 50–70 mm/s |
| Layer height | 0.2mm |
| Support | Len kde nutný |
| Cooling | 30–50% |

### ⚠️ Kritické upozornenia

```
❌ NIKDY nepoužívaj mosadznú trysku na CF filamente → rýchle opotrebenie
✅ Pred tlačou vysušit filament: 65°C / 6 hodín (sušička alebo rúra)
✅ Orientácia ramien pri tlači: VERTIKÁLNE (vrstvy ⊥ na ťahové sily)
✅ Miesta pre skrutky: 100% infill v Bambu Studio (modifier)
```

### Postup pre heat inserts

```
1. Vytlač otvory o 0.2mm menšie ako vonkajší priemer insertu
2. Nahrej spájkovačku na 200°C
3. Polož insert na otvor
4. Pomaly zatlač kolmo – insert sa roztopí do plastu
5. Nechaj vychladnúť 60 sekúnd pred dotykom
```

### Kde stiahnuť modely

| Zdroj | Link | Poznámka |
|---|---|---|
| Printables | printables.com → "7 inch FPV frame" | Zadarmo |
| TBS Source One | team-blacksheep.com | Open-source, zadarmo |
| Thingiverse | thingiverse.com → "drone frame 7" | Zadarmo |
| Cults3D | cults3d.com | Platené, kvalitnejšie |

---

## 🔩 Mechanická zostava

### Postup montáže – krok po kroku

**Krok 1 – Príprava rámu**
```
1. Vytlač všetky diely rámu (ramená, stred, kryty)
2. Vtlač heat inserts do všetkých otvorov pre M3 skrutky
3. Skontroluj všetky diely na trhliny
4. Prebrúš kontaktné plochy (200 grid brúsny papier)
```

**Krok 2 – Montáž motorov**
```
1. Prirav 4x motor 2507
2. Skrutky M3x8 + Loctite Blue
3. Utiahnuť skrutky motorov: 1.5 Nm (krížom)
4. Skontroluj smer závitu hriadeľa:
   - CW motor (clockwise) → CCW matica (M3 ľavý závit)
   - CCW motor → CW matica (M3 pravý závit)
5. Káble motorov nechaj voľné (zapoja sa neskôr)
```

**Krok 3 – FC + ESC Stack**
```
1. Priprav 4x M3 gumové vibration dampeners
2. Vlož spodný ESC na dampeners
3. Stack konektor spoj s FC
4. FC je hore, ESC dole
5. Zafixuj M3 nylonovou maticou (nie príliš utiahnuť!)
6. FC musí byť ROVNOBEŽNE s rámom (skontroluj vizuálne)
```

**Krok 4 – GPS stožiar**
```
1. GPS modul umiestni čo najďalej od FC a motorov
   (minimalizácia magnetického rušenia)
2. Ideálna pozícia: vzadu na teleskopickom stožiari
3. Výška GPS nad rámom: min. 3–5 cm
4. Zafixuj káble plastovými sťahovacími páskami
```

---

## ⚡ Elektrické zapojenie

### Poradie spájkovania

```
1. ESC → kondenzátor (1000µF paralelne na XT60 vstup)
2. ESC → XT60 konektor (batériový vstup)
3. Motory → ESC výstupy (3 drôty, poradie určíme neskôr v softvéri)
4. FC → ESC stack konektor (sériové zapojenie)
5. ELRS RX → FC UART2 (4 drôty: TX, RX, 5V, GND)
6. GPS → FC UART1 + I2C (6 drôtov)
7. DJI O3 → FC UART3 + napájanie
8. WS2812B → FC LED_STRIP pin + 5V + GND
```

### ⚠️ Pravidlá spájkovania

```
✅ Pocínuj plochy pred spájaním (pre-tin)
✅ Krátke spoje = menej rušenia
✅ Hrubšie drôty pre napájanie (18–20 AWG)
✅ Tenšie drôty pre signál (26–28 AWG)
✅ Po každom spoji skontroluj multimetrom (kontinuita)
❌ Nikdy nespájaj pri zapojenej batérii!
❌ Max čas spájkovania na jednom bode: 3 sekundy
```

### Farebné kódovanie káblov

| Farba | Funkcia |
|---|---|
| Červená | +5V / +Bat+ |
| Čierna | GND |
| Biela / Žltá | Signál / Data |
| Modrá | UART TX |
| Zelená | UART RX |

---

## 💻 Konfigurácia softvéru

### Požadovaný softvér (PC/Mac/Linux)

| Softvér | Použitie | Download |
|---|---|---|
| iNav Configurator | Nastavenie FC | github.com/iNavFlight/inav-configurator |
| EdgeTX Companion | Záloha/nastavenie rádia | edgetx.org |
| ELRS Configurator | Flash ELRS firmware | expresslrs.org |
| Betaflight (voliteľne) | Motor test | betaflight.com |
| STM32 DFU drivers | USB pripojenie FC | (Windows only) |

---

## 📻 Nastavenie ovládača EdgeTX

### Priradenie prepínačov na kanály

```
MDL → Inputs → pridaj nové vstupy:

Vstup 1: ARM
  Source: SA (2-polohový)
  Channel: CH5

Vstup 2: Flight Mode
  Source: SB (3-polohový)
  Channel: CH6

Vstup 3: LED
  Source: SD (2-polohový)   ← tlačidlo pre LED
  Channel: CH7

Vstup 4: Buzzer / Beeper
  Source: SE (momentary)
  Channel: CH8
```

### Mixes nastavenie

```
MDL → Mixes:

CH1: Roll    → Input: Aileron (ĽP stick, X)
CH2: Pitch   → Input: Elevator (ĽP stick, Y)
CH3: Throttle→ Input: Throttle (ĽP stick, horná)
CH4: Yaw     → Input: Rudder (ĽP stick, X)
CH5: ARM     → Input: SA
CH6: Mode    → Input: SB
CH7: LED     → Input: SD   ← LED kanál
CH8: Beeper  → Input: SE
```

### Overenie kanálov

```
MDL → Outputs → skontroluj:
- CH7 v polohe OFF (SD dole): hodnota ~1000 µs
- CH7 v polohe ON  (SD hore): hodnota ~2000 µs
```

### Failsafe nastavenie (KRITICKÉ!)

```
MDL → Outputs → každý kanál → [long press] → Failsafe:
  CH1–CH4: Hold (drž poslednú hodnotu)
  CH3 (Throttle): Custom → 1000 µs (motors off)
  CH5 (ARM): Custom → 1000 µs (disarm)
```

---

## 🧭 Konfigurácia iNav

### Krok 1 – Flashovanie firmware

```
1. Otvor iNav Configurator
2. Prepni FC do DFU módu:
   - Podrž BOOT tlačidlo na FC
   - Pripoj USB → pusti tlačidlo
3. Configurator → Firmware Flasher
4. Vyber: SpeedyBee F405 V4
5. Vyber: najnovšia verzia iNav
6. Full Chip Erase: ✅ ÁNO (prvý flash)
7. Klikni [Flash Firmware]
8. Po dokončení: Reboot FC
```

### Krok 2 – Základné nastavenia (Setup tab)

```
Board Alignment:
  Roll:  0°
  Pitch: 0°    (uprav ak FC nie je priamo zarovnaný)
  Yaw:   0°

Accelerometer Calibration:
  Polož dron na rovný povrch
  Klikni [Calibrate Accelerometer]
  Nechaj 5 sekúnd nehybne
```

### Krok 3 – Porty (Ports tab)

| Port | Funkcia | Baudrate |
|---|---|---|
| UART1 | GPS | 57600 |
| UART2 | Serial RX (ELRS) | 420000 |
| UART3 | MSP (DJI O3) | 115200 |
| USB | MSP | – |

### Krok 4 – Konfigurácia (Configuration tab)

```
ESC/Motor:
  Protocol: DSHOT600
  Motor Poles: 14 (pre 2507 motor)
  Min Throttle: 1070
  Max Throttle: 2000

Receiver:
  Type: Serial (via UART)
  Protocol: CRSF (pre ELRS)

GPS:
  Provider: UBLOX
  SBAS: Auto
  Baud: 57600

Magnetometer:
  Enable: ✅ ÁNO
  Device: automaticky (BN-880)

Barometer:
  Enable: ✅ ÁNO

Features:
  ✅ GPS
  ✅ TELEMETRY
  ✅ LED_STRIP
  ✅ OSD
```

### Krok 5 – PID a Filter (Záložka PID Tuning)

```
Prednastavené hodnoty pre 7" long range:

Roll:  P=45  I=60  D=20  FF=90
Pitch: P=47  I=65  D=22  FF=95
Yaw:   P=50  I=80  D=0   FF=100

Master Multiplier: 1.0
(Doladiť po prvých letoch)

Filters:
  Gyro LPF: 100Hz
  D-term LPF: 100Hz
```

### Krok 6 – Navigačné módy (Modes tab)

```
ARM:          AUX1 (CH5)  | 1800–2100 µs
NAV POSHOLD:  AUX2 (CH6)  | 1300–1700 µs (SB stred)
NAV RTH:      AUX2 (CH6)  | 1800–2100 µs (SB hore)
ANGLE:        AUX2 (CH6)  | 1000–1300 µs (SB dole)
LED:          AUX3 (CH7)  | 1800–2100 µs  ← LED tlačidlo!
BEEPER:       AUX4 (CH8)  | 1800–2100 µs
```

### Krok 7 – GPS a RTH nastavenia (CLI)

```
# Otvor CLI záložku, vlož tieto príkazy:

set nav_rth_altitude = 5000        # RTH výška: 50m (v cm)
set nav_rth_climb_first = ON        # Najprv vystúp, potom letí domov
set nav_rth_tail_first = OFF
set nav_min_rth_distance = 500      # Min. 5m od home pre RTH
set failsafe_procedure = RTH        # Pri strate signálu → RTH
set failsafe_throttle_low_delay = 100
set nav_wp_radius = 200             # GPS waypoint radius: 2m

save
```

### Krok 8 – OSD nastavenie

```
OSD záložka → zapni tieto prvky:

✅ GPS Coordinates (súradnice)
✅ GPS Speed
✅ Home Direction (šípka domov) ← KRITICKÉ pre 5km!
✅ Home Distance (vzdialenosť od domova)
✅ Altitude
✅ Battery Voltage
✅ Battery Current
✅ mAh Used (spotrebované mAh)
✅ Fly Time (čas letu)
✅ RSSI / Link Quality
✅ Warnings (varovania)
```

---

## 💡 Nastavenie LED

### Hardware – zapojenie WS2812B

```
FC (LED_STRIP pin) ──────── DIN (LED 1) ─── DOUT ──── DIN (LED 2)
FC (5V)           ──────┬── VCC (LED 1)
                        └── VCC (LED 2)
FC (GND)          ──────┬── GND (LED 1)
                        └── GND (LED 2)
```

### iNav CLI – konfigurácia LED

```bash
# Otvor CLI v iNav Configurator a vlož:

# LED 0: ľavá strana, biela farba pri zapnutí
led 0 0,0::FO:0

# LED 1: pravá strana, biela farba pri zapnutí
led 1 1,0::FO:0

# Farba 0 = biela (H=0, S=0, V=255)
color 0 0,0,255

# Ulož nastavenia
save
```

### EdgeTX – priradenie tlačidla

```
Na ovládači (RadioMaster):
  SD prepínač (2-polohový) → CH7 (AUX3)

  SD = DOLE  → CH7 = ~1000 µs → LED VYPNUTÉ
  SD = HORE  → CH7 = ~2000 µs → LED ZAPNUTÉ
```

### iNav Modes – aktivácia LED

```
Záložka Modes:
  LED → AUX3 → rozsah: 1800–2100 µs
  [Save]
```

### Test LED (bez letu)

```
1. Zapni ovládač
2. Pripoj FC cez USB (bez batérie)
3. Prepni SD prepínač do polohy HORE
4. LED musia zasviatiť bielou farbou ✅
5. Prepni SD dole → LED zhasnú ✅
```

---

## ✅ Testovanie

### Fáza 1 – Bench test (na stole, BEZ vrtúľ)

```
Test 1: Napájanie
  □ Pripoj batériu
  □ Skontroluj: FC sa rozblikala (bootovanie)
  □ Skontroluj: DJI O3 sa zapla (zelená LED)
  □ Skontroluj: GPS bliká (hľadá fix)
  □ Multimetrom: 5V na BEC výstupe ±0.2V

Test 2: RC Link
  □ Zapni ovládač (EdgeTX)
  □ V iNav: záložka Receiver → pohyb stickmi
  □ CH1–CH4 reagujú na pohyb
  □ CH5 (ARM): SA prepínač zmení hodnotu
  □ CH7 (LED): SD prepínač zmení hodnotu

Test 3: Motory (BEZ VRTÚĽ!)
  □ iNav → Motors záložka
  □ Zaškrtni "I understand the risks"
  □ Master slider pomaly na ~10%
  □ Všetky 4 motory sa točia ✅
  □ Skontroluj smer každého motora (rukou jemne zastav)

Test 4: Smer motorov
  □ M1 (predný pravý): CW (po hodinách)
  □ M2 (predný ľavý): CCW (proti hodinám)
  □ M3 (zadný ľavý): CW
  □ M4 (zadný pravý): CCW
  □ Ak smer nesedí → prehoď 2 ľubovoľné drôty na motore

Test 5: LED
  □ Prepni SD na ovládači
  □ LED zasvietia bielou ✅

Test 6: GPS
  □ Vynes dron von (alebo k oknu)
  □ Počkaj na GPS fix: min. 6 satelitov
  □ iNav → záložka Setup → GPS súradnice ✅
  □ Home bod sa uloží pri prvom ARM
```

### Fáza 2 – Motor spin test (s vrtulami, v ruke)

```
⚠️ POZOR: Vrtule sú nebezpečné! Dron drž pevne, ďalej od tela!

□ Nasaď vrtule (CW na CW motory, CCW na CCW)
□ ARM dron (SA hore)
□ Throttle minimálne zvýš na ~5%
□ Dron by mal ťahovať HORE (nie bokom)
□ Skontroluj vibrácie – ak silné, skontroluj vrtule/motory
□ DISARM okamžite
```

### Fáza 3 – Hover test (prvý let)

```
□ Vyber otvorené priestranstvo (min. 20m okolo)
□ GPS fix: min. 8 satelitov
□ Skontroluj batériu: plná (25.2V pre 6S)
□ Nastav RTH výšku: 20m (pre prvý test)
□ ARM, pomaly zvyšuj throttle
□ Hover na 1m výšky, 30 sekúnd
□ Skontroluj stabilitu – dron by nemal driftovať
□ Otestuj POSHOLD (SB stred) – dron drží pozíciu ✅
□ LAND, DISARM
□ Skontroluj motory na teplotu (max 60°C)
```

### Fáza 4 – RTH test

```
□ Vzlietni na 20m výšku
□ Odleť 50m od miesta vzletu
□ Prepni SB do hornej polohy (RTH mód)
□ Dron sa musí otočiť a letieť späť ✅
□ Pristátie na mieste vzletu (±2m) ✅
□ Ak RTH nefunguje → skontroluj GPS fix a magnetometer
```

### Fáza 5 – Dosah test

```
□ Začni na 500m, skontroluj RSSI/LQ v OSD
□ Postupne zväčšuj dosah: 500m → 1km → 2km → 5km
□ LQ (Link Quality) nesmie klesnúť pod 70%
□ RSSI nesmie klesnúť pod -100 dBm
□ Sleduj batériu: pristaj pri 3.6V/článok (21.6V celkom)
□ Nechaj vždy 30% batérie ako rezervu na RTH!
```

---

## ⚖️ Hmotnostný rozpočet

| Komponent | Hmotnosť |
|---|---|
| Rám 7" (PETG-CF tlačený) | 220g |
| 4x Motory 2507 | 180g |
| FC + ESC Stack | 65g |
| GPS modul BN-880 | 20g |
| ELRS Nano RX | 5g |
| DJI O3 Air Unit | 125g |
| Anténa RC + video | 20g |
| WS2812B LED + káble | 10g |
| Kondenzátor, XT60 | 15g |
| Skrutky, heat inserts | 20g |
| Vrtule 7" (4ks) | 25g |
| Káble napájacie | 30g |
| **Dron BEZ batérie** | **~735g** |
| Batéria 6S 4000mAh | 370g |
| **Dron S batériou** | **~1105g** |
| Payload (200g) | 200g |
| **CELKOVÁ VÁHA** | **~1305g** |

### Thrust-to-weight ratio

```
4x Motor 2507 @ 6S s 7" vrtulami:
  Ťah každého motora: ~900g
  Celkový ťah: 4 × 900g = 3600g

Thrust ratio: 3600g / 1305g = 2.76:1  ✅
(Minimum pre stabilný let: 2:1)
```

---

## 🗺️ Legislatíva SR

| Požiadavka | Detail | Kde vybaviť |
|---|---|---|
| Registrácia pilota | Povinná (dron nad 250g) | caa.sk |
| Preukaz pilota A2 | Pre dron 900g–4kg | online kurz + test |
| Registrácia dronu | Evidenčné číslo na drona | caa.sk |
| Poistenie | Zodpovednosť za škody | ľubovoľná poisťovňa |
| BVLOS povolenie | Let za priamou viditeľnosťou (5km) | Dopravný úrad SR |
| VTX výkon | Max 25mW na 5.8GHz bez licencie | – |
| HAM licencia | Pre 900MHz TX nad limit | hamradio.sk |

> ⚠️ **Let na 5km = BVLOS** (Beyond Visual Line of Sight). Vyžaduje **špeciálne povolenie** od Dopravného úradu SR. Bez povolenia musíš mať dron vždy v priamom dohľade!

---

## 🔍 Troubleshooting

| Problém | Príčina | Riešenie |
|---|---|---|
| Motor sa netočí | Zlé zapojenie ESC | Skontroluj 3 drôty motora |
| Motor točí nesprávnym smerom | Poradie drôtov | Prehoď ľubovoľné 2 drôty |
| GPS nezdvíha fix | Rušenie od FC | Presun GPS ďalej od FC |
| ELRS sa nepripája | Binding | Znovu spusti binding procedúru |
| Dron driftuje v POSHOLD | Nekalibrovaný kompas | Kalibrácia kompasu v iNav |
| LED nereagujú | Zlý pin alebo mód | Skontroluj LED_STRIP pin a iNav Modes |
| Vibrácie pri lete | Nevyvážené vrtule | Vymeň vrtule, skontroluj motory |
| Krátky čas letu | Príliš agresívne PID | Zníž PID values, leti pomalšie |
| RTH nefunguje | Žiadny GPS fix pri ARM | Čakaj na 8+ satelitov pred ARM |
| OSD nezobrazuje | UART nastavenie | Skontroluj UART3 pre DJI O3 |

---

## 📁 Štruktúra projektu

```
fpv-drone/
├── README.md                  ← tento súbor
├── hardware/
│   ├── frame/                 ← STL súbory rámu
│   ├── wiring_diagram.pdf     ← schéma zapojenia
│   └── parts_list.csv         ← nákupný zoznam
├── firmware/
│   ├── inav_config.txt        ← iNav CLI dump
│   └── edgetx_model.yml       ← EdgeTX model backup
├── docs/
│   ├── flight_test_log.md     ← záznam testov
│   └── maiden_flight.md       ← prvý let
└── photos/
    └── build_photos/          ← fotky zo zostavenia
```

---

## 📜 Licencia

MIT License – voľné použitie, modifikácia a distribúcia.

---

## 👤 Autor

Vytvorené pre komunitu FPV nadšencov na Slovensku 🇸🇰

> **Disclaimer:** Autor nezodpovedá za škody spôsobené zostavením alebo prevádzkou dronu. Vždy lietaj zodpovedne a v súlade s platnou legislatívou SR.
