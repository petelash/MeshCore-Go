# MeshCore Go

**English** · [Hrvatski](#hrvatski)

Android client for [MeshCore](https://meshcore.co.uk) LoRa mesh networks.

**MeshCore Go is a complete, everyday MeshCore app** – you use it exactly like the official MeshCore app: connect your companion node over **Bluetooth LE, USB or WiFi**, chat in channels and direct messages, see nodes on the map, manage repeaters and room servers. It **works with every MeshCore companion node**, whether you carry it with you or keep it on your desk.

**On top of that it has one extra feature**, the reason this app was made: a **built-in Tailscale VPN**. With it you can use your MeshCore node from anywhere over the internet while the node itself stays at home (see below). You don't have to use it – without Tailscale the app works like any other MeshCore client.

## Leave the node at home, take MeshCore with you
Your node can stay at home – on the roof, by the window or wherever it has the best coverage – connected to WiFi and power. Thanks to the **built-in Tailscale VPN**, the app reaches it from anywhere over the internet (mobile data or any WiFi), so you can read and send MeshCore messages, see the map and manage the node **without carrying the node with you**.

- No port forwarding and no public IP needed: Tailscale creates a private, encrypted connection between your phone and your home network.
- At home the app talks to the node directly over WiFi; away from home it switches to Tailscale by itself.
- The node stays where its antenna works best and keeps receiving messages while you are away.

**What you need today:** a free [Tailscale](https://tailscale.com) account, a WiFi companion node and, at home, a device that is always on and acts as a Tailscale *subnet router* (e.g. a Raspberry Pi, a NAS or a router with Tailscale), so the app can reach the node's home IP address.

### Coming soon: firmware with Tailscale built in
Custom MeshCore companion firmware for the **Seeed Studio XIAO ESP32S3 + Wio-SX1262** with the **Tailscale VPN integrated directly in the node** will be published soon. The node will join your tailnet by itself, so **no extra computer or subnet router at home will be needed** – just the node, WiFi and power.

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
MeshCore Go © 2026 Marinko Vrbanić, released under the **[MIT licence](LICENSE)**.
You may freely use, copy, modify and share it, as long as you keep the copyright notice and the licence text.
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

Android klijent za [MeshCore](https://meshcore.co.uk) LoRa mesh mreže.

**MeshCore Go je potpuna MeshCore aplikacija za svakodnevno korištenje** – koristiš je isto kao službenu MeshCore aplikaciju: spajaš companion node preko **Bluetootha LE, USB-a ili WiFi-ja**, dopisuješ se u kanalima i privatnim porukama, gledaš nodeove na karti, upravljaš repetitorima i chat sobama. **Radi sa svim MeshCore companion nodeovima**, bilo da node nosiš sa sobom ili ti stoji na stolu.

**Uz to ima jednu dodatnu mogućnost**, zbog koje je aplikacija i nastala: **ugrađeni Tailscale VPN**. S njim svoj MeshCore node možeš koristiti s bilo kojeg mjesta preko interneta, a node pritom ostaje kod kuće (vidi niže). Ne moraš ga koristiti – bez Tailscalea aplikacija radi kao i svaki drugi MeshCore klijent.

## Node ostaje doma, MeshCore ide s tobom
Node može ostati kod kuće – na krovu, uz prozor ili gdje god ima najbolje pokrivanje – spojen na WiFi i napajanje. Zahvaljujući **ugrađenom Tailscale VPN-u** aplikacija do njega dolazi s bilo kojeg mjesta preko interneta (mobilni podaci ili bilo koji WiFi), pa možeš čitati i slati MeshCore poruke, gledati kartu i upravljati nodeom **bez nošenja nodea sa sobom**.

- Ne treba otvarati portove na routeru ni imati javnu IP adresu: Tailscale radi privatnu, šifriranu vezu između mobitela i kućne mreže.
- Kod kuće se aplikacija spaja na node izravno preko WiFi-ja, a izvan kuće sama prelazi na Tailscale.
- Node ostaje tamo gdje mu antena najbolje radi i prima poruke i dok tebe nema.

**Što je danas potrebno:** besplatan [Tailscale](https://tailscale.com) račun, WiFi companion node i kod kuće uređaj koji je stalno uključen i služi kao Tailscale *subnet router* (npr. Raspberry Pi, NAS ili router s Tailscaleom), da aplikacija dođe do kućne IP adrese nodea.

### Uskoro: firmware s ugrađenim Tailscaleom
Uskoro će biti objavljen prilagođeni MeshCore companion firmware za **Seeed Studio XIAO ESP32S3 + Wio-SX1262** s **Tailscale VPN-om integriranim izravno u node**. Node će se sam spojiti u tvoj tailnet, pa **kod kuće neće trebati dodatno računalo ni subnet router** – samo node, WiFi i napajanje.

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
MeshCore Go © 2026 Marinko Vrbanić, objavljeno pod **[MIT licencom](LICENSE)**.
Aplikaciju smiješ slobodno koristiti, kopirati, mijenjati i dijeliti, uz uvjet da zadržiš navod autora i tekst licence.
Aplikacija se daje **„kakva jest”, bez ikakvog jamstva**; autor ne odgovara za štetu nastalu njezinim korištenjem.

Neslužbeni klijent – nije povezan s MeshCore projektom ni s tvrtkom Tailscale Inc. MeshCore i Tailscale pripadaju svojim vlasnicima.

Komponente otvorenog koda i njihove licence navedene su u tablici iznad (engleski dio) i u aplikaciji: Postavke → O aplikaciji → Licenca.
