# MeshCore Go

**English** · [Hrvatski](#hrvatski)

Android client for [MeshCore](https://meshcore.co.uk) LoRa mesh nodes, with **Tailscale built in**: at home it talks to your WiFi companion node directly, away from home it reaches the same node through your tailnet. Nothing to switch.

This repository only holds the **releases** (APK files). The source code is not public.

## Features
- Connect over WiFi (TCP, LAN or Tailscale), Bluetooth LE or USB
- Direct messages, channels and room servers; delivery status and retries (direct / flood)
- Message routes on the map, repeaters that heard your channel message
- DM route control (automatic, always flood, manual path)
- Region scope (default on the node and per channel)
- Notifications per channel and per contact, received adverts, repeater admin (status, telemetry, CLI)
- Map with MeshCore node symbols, light / dark / AMOLED theme
- Languages: Croatian, Serbian, English, German
- Built-in update check

## Download and install
1. Open **[Releases](../../releases/latest)** and download the APK for your phone:
   - `…-arm64.apk` – almost all phones from the last years (recommended)
   - `…-armv7.apk` – older 32-bit phones
   - `…-universal.apk` – if you are not sure (larger)
2. Open the file and allow "Install unknown apps" for your browser or file manager when Android asks.

## Updates
The app checks this repository once a day (Settings → About → *Check for updates*, can be turned off). When a newer version exists it offers to download it; Android then asks you to confirm the install. Your messages and settings stay.

## Licence
MeshCore Go © 2026 Marinko Vrbanić. **All rights reserved.**
The app is free for personal and non-commercial use. Selling it or publishing modified versions without the author's permission is not allowed.
The app is provided **"as is", without any warranty**; the author is not liable for any damage arising from its use.

Unofficial client – not affiliated with the MeshCore project or Tailscale Inc. MeshCore and Tailscale belong to their owners.

### Open-source components
| Component | Licence |
|---|---|
| Tailscale (tsnet) | BSD-3-Clause |
| Go mobile (gomobile) | BSD-3-Clause |
| osmdroid | Apache License 2.0 |
| usb-serial-for-android | MIT |
| AndroidX, Jetpack Compose, Kotlin, kotlinx.coroutines | Apache License 2.0 |
| MeshCore Map – node symbols (map.meshcore.dev), © 2025 Rastislav Vysoky | MIT |
| Map data © OpenStreetMap contributors | ODbL |

---

<a id="hrvatski"></a>
# MeshCore Go (hrvatski)

Android klijent za [MeshCore](https://meshcore.co.uk) LoRa mesh nodeove s **ugrađenim Tailscaleom**: kod kuće se spaja izravno na tvoj WiFi companion node, a izvan kuće do istog nodea dolazi preko tvog tailneta. Ništa ne treba prebacivati.

Ovaj repozitorij sadrži samo **izdanja** (APK datoteke). Izvorni kod nije javan.

## Mogućnosti
- Spajanje preko WiFi-ja (TCP, LAN ili Tailscale), Bluetootha LE ili USB-a
- Privatne poruke, kanali i chat sobe; status isporuke i ponovni pokušaji (direktno / flood)
- Putanje poruka na karti, repetitori koji su čuli tvoju poruku u kanalu
- Kontrola rute za DM (automatski, uvijek flood, ručna putanja)
- Scope regija (zadani na nodeu i po kanalu)
- Obavijesti po kanalu i po kontaktu, primljeni adverti, administracija repetitora (status, telemetrija, CLI)
- Karta sa simbolima MeshCore nodeova, svijetla / tamna / AMOLED tema
- Jezici: hrvatski, srpski, engleski, njemački
- Ugrađena provjera ažuriranja

## Preuzimanje i instalacija
1. Otvori **[Releases](../../releases/latest)** i preuzmi APK za svoj mobitel:
   - `…-arm64.apk` – gotovo svi mobiteli iz zadnjih godina (preporučeno)
   - `…-armv7.apk` – stariji 32-bitni mobiteli
   - `…-universal.apk` – ako nisi siguran (veći)
2. Otvori datoteku i dopusti "Instaliraj nepoznate aplikacije" za preglednik ili upravitelj datoteka kad Android to zatraži.

## Ažuriranja
Aplikacija jednom dnevno provjerava ovaj repozitorij (Postavke → O aplikaciji → *Provjeri ažuriranje*, može se isključiti). Kad postoji novija verzija, ponudi preuzimanje, a Android zatim traži da potvrdiš instalaciju. Poruke i postavke ostaju.

## Licenca
MeshCore Go © 2026 Marinko Vrbanić. **Sva prava pridržana.**
Aplikacija je besplatna za osobnu i nekomercijalnu upotrebu. Nije dopušteno prodavati je ni objavljivati izmijenjene verzije bez dopuštenja autora.
Aplikacija se daje **„kakva jest”, bez ikakvog jamstva**; autor ne odgovara za štetu nastalu njezinim korištenjem.

Neslužbeni klijent – nije povezan s MeshCore projektom ni s tvrtkom Tailscale Inc. MeshCore i Tailscale pripadaju svojim vlasnicima.

Komponente otvorenog koda i njihove licence navedene su u tablici iznad (engleski dio) i u aplikaciji: Postavke → O aplikaciji → Licenca.
