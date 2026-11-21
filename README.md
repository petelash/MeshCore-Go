# MeshCore Go

**English** · [Hrvatski](#hrvatski) · [Magyar](#magyar)

Android client for [MeshCore](https://meshcore.co.uk) LoRa mesh networks.

> 🔗 **Companion project:** MeshCore Go is closely tied to **[MeshCore Tailscale Companion](https://github.com/petelash/meshcore-tailscale-companion)**, our companion firmware with Tailscale built into the node. Using that firmware with this app is recommended.

> ### 👉 [Web flasher: put Tailscale VPN on your node](https://petelash.github.io/meshcore-tailscale-companion/)
> With the **[web flasher](https://petelash.github.io/meshcore-tailscale-companion/)** you install the MeshCore Tailscale Companion firmware on a **Seeed Studio XIAO ESP32S3 + Wio-SX1262** in one click (Chrome or Edge on a computer, USB cable).
> The firmware has the **Tailscale VPN built into the node**: the node joins your private, encrypted tailnet by itself and gets a 100.x.x.x address.
> MeshCore Go, with its own built-in Tailscale, then reaches the node **from anywhere over the internet** (mobile data or any WiFi) – no subnet router,
> no Raspberry Pi, no port forwarding and no public IP. The same page also updates the firmware later, keeping all settings.

**MeshCore Go is a complete, everyday MeshCore app** – you use it exactly like the official MeshCore app: connect your companion node over **Bluetooth LE, USB or WiFi**, chat in channels and direct messages, see nodes on the map, manage repeaters and room servers. It **works with every MeshCore companion node**, whether you carry it with you or keep it on your desk.

**On top of that it has one extra feature**, the reason this app was made: a **built-in Tailscale VPN**. With it you can use your MeshCore node from anywhere over the internet while the node itself stays at home (see below). You don't have to use it – without Tailscale the app works like any other MeshCore client.

## Leave the node at home, take MeshCore with you
Your node can stay at home – on the roof, by the window or wherever it has the best coverage – connected to WiFi and power. Thanks to the **built-in Tailscale VPN**, the app reaches it from anywhere over the internet (mobile data or any WiFi), so you can read and send MeshCore messages, see the map and manage the node **without carrying the node with you**.

- No port forwarding and no public IP needed: Tailscale creates a private, encrypted connection between your phone and your home network.
- At home the app talks to the node directly over WiFi; away from home it switches to Tailscale by itself.
- The node stays where its antenna works best and keeps receiving messages while you are away.

**What you need:** a free [Tailscale](https://tailscale.com) account and a WiFi companion node. With the recommended [MeshCore Tailscale Companion](https://github.com/petelash/meshcore-tailscale-companion) firmware nothing else is needed. With other WiFi firmware you also need, at home, a device that is always on and acts as a Tailscale *subnet router* (e.g. a Raspberry Pi, a NAS or a router with Tailscale), so the app can reach the node's home IP address.

## Recommended firmware: MeshCore Tailscale Companion
MeshCore Go and **[MeshCore Tailscale Companion](https://github.com/petelash/meshcore-tailscale-companion)** are two parts of the same project and work best together.

- The firmware runs on the **Seeed Studio XIAO ESP32S3 + Wio-SX1262** and has the **Tailscale VPN built directly into the node**.
- The node joins your tailnet by itself and gets a 100.x.x.x address, so **no extra computer or subnet router is needed at home** – just the node, WiFi and power.
- In MeshCore Go open Tailscale → *Devices in the tailnet* and tap the node to connect to it.
- Install and update it with one click in the **[web flasher](https://petelash.github.io/meshcore-tailscale-companion/)** (Chrome or Edge on a computer).

We recommend this firmware for using MeshCore Go over Tailscale. The app still works with every other MeshCore companion firmware.

This repository only holds the **releases** (APK files). The source code is not public.

## Features
- Connect over WiFi (TCP, LAN or Tailscale), Bluetooth LE or USB
- Direct messages, channels and room servers; delivery status and retries (direct / flood)
- Message routes on the map, repeaters that heard your channel message
- DM route control (automatic, always flood, manual path)
- Region scope (default on the node and per channel)
- Notifications per channel and per contact, received adverts, repeater admin (status, telemetry, CLI)
- Map with MeshCore node symbols, light / dark / AMOLED theme
- Languages: Croatian, Serbian, English, German, Hungarian
- Built-in update check

## Download and install
1. Open **[Releases](../../releases/latest)** and download the APK for your phone:
   - `…-arm64.apk` – almost all phones from the last years (recommended)
   - `…-armv7.apk` – older 32-bit phones
   - `…-universal.apk` – if you are not sure (larger)
2. Open the file and allow "Install unknown apps" for your browser or file manager when Android asks.

## Updates
What changed in each version: **[CHANGELOG](CHANGELOG.md)**.

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
| Fonts: Open Sans, Montserrat, Poppins, Inter, Nunito, Raleway, Rubik (Google Fonts) | SIL Open Font License 1.1 |
| Font: Roboto Slab (Google Fonts) | Apache License 2.0 |

---

<a id="hrvatski"></a>
# MeshCore Go (hrvatski)

Android klijent za [MeshCore](https://meshcore.co.uk) LoRa mesh mreže.

> 🔗 **Povezani projekt:** MeshCore Go usko je povezan s našim projektom **[MeshCore Tailscale Companion](https://github.com/petelash/meshcore-tailscale-companion)**, companion firmwareom s Tailscaleom ugrađenim u sam node. Preporučuje se korištenje tog firmwarea s ovom aplikacijom.

> ### 👉 [Web flasher: Tailscale VPN na tvom nodeu](https://petelash.github.io/meshcore-tailscale-companion/)
> Preko **[web flashera](https://petelash.github.io/meshcore-tailscale-companion/)** jednim klikom instaliraš firmware MeshCore Tailscale Companion na **Seeed Studio XIAO ESP32S3 + Wio-SX1262** (Chrome ili Edge na računalu, USB kabel).
> Firmware ima **Tailscale VPN ugrađen u sam node**: node se sam spoji u tvoju privatnu, šifriranu mrežu (tailnet) i dobije 100.x.x.x adresu.
> MeshCore Go, koji ima svoj ugrađeni Tailscale, tada do nodea dolazi **s bilo kojeg mjesta preko interneta** (mobilni podaci ili bilo koji WiFi) – bez subnet routera,
> bez Raspberry Pi-ja, bez otvaranja portova i bez javne IP adrese. Na istoj stranici firmware kasnije i nadograđuješ, uz zadržavanje svih postavki.

**MeshCore Go je potpuna MeshCore aplikacija za svakodnevno korištenje** – koristiš je isto kao službenu MeshCore aplikaciju: spajaš companion node preko **Bluetootha LE, USB-a ili WiFi-ja**, dopisuješ se u kanalima i privatnim porukama, gledaš nodeove na karti, upravljaš repetitorima i chat sobama. **Radi sa svim MeshCore companion nodeovima**, bilo da node nosiš sa sobom ili ti stoji na stolu.

**Uz to ima jednu dodatnu mogućnost**, zbog koje je aplikacija i nastala: **ugrađeni Tailscale VPN**. S njim svoj MeshCore node možeš koristiti s bilo kojeg mjesta preko interneta, a node pritom ostaje kod kuće (vidi niže). Ne moraš ga koristiti – bez Tailscalea aplikacija radi kao i svaki drugi MeshCore klijent.

## Node ostaje doma, MeshCore ide s tobom
Node može ostati kod kuće – na krovu, uz prozor ili gdje god ima najbolje pokrivanje – spojen na WiFi i napajanje. Zahvaljujući **ugrađenom Tailscale VPN-u** aplikacija do njega dolazi s bilo kojeg mjesta preko interneta (mobilni podaci ili bilo koji WiFi), pa možeš čitati i slati MeshCore poruke, gledati kartu i upravljati nodeom **bez nošenja nodea sa sobom**.

- Ne treba otvarati portove na routeru ni imati javnu IP adresu: Tailscale radi privatnu, šifriranu vezu između mobitela i kućne mreže.
- Kod kuće se aplikacija spaja na node izravno preko WiFi-ja, a izvan kuće sama prelazi na Tailscale.
- Node ostaje tamo gdje mu antena najbolje radi i prima poruke i dok tebe nema.

**Što je potrebno:** besplatan [Tailscale](https://tailscale.com) račun i WiFi companion node. Uz preporučeni firmware [MeshCore Tailscale Companion](https://github.com/petelash/meshcore-tailscale-companion) ništa drugo ne treba. S drugim WiFi firmwareom kod kuće treba i uređaj koji je stalno uključen i služi kao Tailscale *subnet router* (npr. Raspberry Pi, NAS ili router s Tailscaleom), da aplikacija dođe do kućne IP adrese nodea.

## Preporučeni firmware: MeshCore Tailscale Companion
MeshCore Go i **[MeshCore Tailscale Companion](https://github.com/petelash/meshcore-tailscale-companion)** dva su dijela istog projekta i najbolje rade zajedno.

- Firmware radi na **Seeed Studio XIAO ESP32S3 + Wio-SX1262** i ima **Tailscale VPN ugrađen izravno u node**.
- Node se sam spoji u tvoj tailnet i dobije 100.x.x.x adresu, pa **kod kuće ne treba dodatno računalo ni subnet router** – samo node, WiFi i napajanje.
- U MeshCore Go otvori Tailscale → *Uređaji u tailnetu* i dodirni node da se spojiš na njega.
- Instalira se i nadograđuje jednim klikom u **[web flasheru](https://petelash.github.io/meshcore-tailscale-companion/)** (Chrome ili Edge na računalu).

Za korištenje MeshCore Go preko Tailscalea preporučujemo ovaj firmware. Aplikacija i dalje radi sa svim ostalim MeshCore companion firmwareima.

Ovaj repozitorij sadrži samo **izdanja** (APK datoteke). Izvorni kod nije javan.

## Mogućnosti
- Spajanje preko WiFi-ja (TCP, LAN ili Tailscale), Bluetootha LE ili USB-a
- Privatne poruke, kanali i chat sobe; status isporuke i ponovni pokušaji (direktno / flood)
- Putanje poruka na karti, repetitori koji su čuli tvoju poruku u kanalu
- Kontrola rute za DM (automatski, uvijek flood, ručna putanja)
- Scope regija (zadani na nodeu i po kanalu)
- Obavijesti po kanalu i po kontaktu, primljeni adverti, administracija repetitora (status, telemetrija, CLI)
- Karta sa simbolima MeshCore nodeova, svijetla / tamna / AMOLED tema
- Jezici: hrvatski, srpski, engleski, njemački, mađarski
- Ugrađena provjera ažuriranja

## Preuzimanje i instalacija
1. Otvori **[Releases](../../releases/latest)** i preuzmi APK za svoj mobitel:
   - `…-arm64.apk` – gotovo svi mobiteli iz zadnjih godina (preporučeno)
   - `…-armv7.apk` – stariji 32-bitni mobiteli
   - `…-universal.apk` – ako nisi siguran (veći)
2. Otvori datoteku i dopusti "Instaliraj nepoznate aplikacije" za preglednik ili upravitelj datoteka kad Android to zatraži.

## Ažuriranja
Što se mijenjalo u svakoj verziji: **[popis promjena](CHANGELOG.md#hrvatski)**.

Aplikacija jednom dnevno provjerava ovaj repozitorij (Postavke → O aplikaciji → *Provjeri ažuriranje*, može se isključiti). Kad postoji novija verzija, ponudi preuzimanje, a Android zatim traži da potvrdiš instalaciju. Poruke i postavke ostaju.

## Licenca
MeshCore Go © 2026 Marinko Vrbanić, objavljeno pod **[MIT licencom](LICENSE)**.
Aplikaciju smiješ slobodno koristiti, kopirati, mijenjati i dijeliti, uz uvjet da zadržiš navod autora i tekst licence.
Aplikacija se daje **„kakva jest”, bez ikakvog jamstva**; autor ne odgovara za štetu nastalu njezinim korištenjem.

Neslužbeni klijent – nije povezan s MeshCore projektom ni s tvrtkom Tailscale Inc. MeshCore i Tailscale pripadaju svojim vlasnicima.

Komponente otvorenog koda i njihove licence navedene su u tablici iznad (engleski dio) i u aplikaciji: Postavke → O aplikaciji → Licenca.

---

<a id="magyar"></a>
# MeshCore Go (magyar)

Android kliens [MeshCore](https://meshcore.co.uk) LoRa mesh hálózatokhoz.

> 🔗 **Kapcsolódó projekt:** a MeshCore Go szorosan kapcsolódik a **[MeshCore Tailscale Companion](https://github.com/petelash/meshcore-tailscale-companion)** projekthez, a saját companion firmware-ünkhöz, amelyben a Tailscale magába a node-ba van beépítve. Ezzel az alkalmazással ennek a firmware-nek a használata ajánlott.

> ### 👉 [Webes flasher: Tailscale VPN a node-odra](https://petelash.github.io/meshcore-tailscale-companion/)
> A **[webes flasherrel](https://petelash.github.io/meshcore-tailscale-companion/)** egy kattintással telepítheted a MeshCore Tailscale Companion firmware-t egy **Seeed Studio XIAO ESP32S3 + Wio-SX1262** eszközre (Chrome vagy Edge számítógépen, USB-kábel).
> A firmware-ben a **Tailscale VPN magába a node-ba van beépítve**: a node magától csatlakozik a privát, titkosított tailnetedhez, és 100.x.x.x címet kap.
> A saját beépített Tailscale-jével a MeshCore Go ezután **bárhonnan, az interneten keresztül** eléri a node-ot (mobilnet vagy bármilyen WiFi) – subnet router,
> Raspberry Pi, porttovábbítás és nyilvános IP-cím nélkül. Ugyanezen az oldalon később a firmware-t is frissítheted, minden beállítás megmarad.

**A MeshCore Go teljes értékű, mindennapi MeshCore alkalmazás** – pontosan úgy használod, mint a hivatalos MeshCore alkalmazást: **Bluetooth LE-n, USB-n vagy WiFi-n** csatlakoztatod a companion node-odat, csevegsz csatornákon és közvetlen üzenetekben, látod a node-okat a térképen, kezeled az átjátszókat és a room servereket. **Minden MeshCore companion node-dal működik**, akár magadnál hordod, akár az asztalodon áll.

**Ezen felül van egy extra funkciója**, amiért az alkalmazás készült: a **beépített Tailscale VPN**. Ezzel a MeshCore node-odat bárhonnan használhatod az interneten keresztül, miközben maga a node otthon marad (lásd lent). Nem kötelező használni – Tailscale nélkül az alkalmazás ugyanúgy működik, mint bármely más MeshCore kliens.

## A node otthon marad, a MeshCore veled jön
A node otthon maradhat – a tetőn, az ablak mellett vagy ahol a legjobb a lefedettsége –, WiFi-re és áramra kötve. A **beépített Tailscale VPN-nek** köszönhetően az alkalmazás bárhonnan eléri az interneten keresztül (mobilnet vagy bármilyen WiFi), így olvashatod és küldheted a MeshCore üzeneteket, nézheted a térképet és kezelheted a node-ot **anélkül, hogy magadnál hordanád**.

- Nincs szükség porttovábbításra és nyilvános IP-címre: a Tailscale privát, titkosított kapcsolatot hoz létre a telefonod és az otthoni hálózatod között.
- Otthon az alkalmazás közvetlenül WiFi-n beszél a node-dal, otthonon kívül pedig magától átvált Tailscale-re.
- A node ott marad, ahol az antennája a legjobban működik, és a távollétedben is fogadja az üzeneteket.

**Amire szükséged van:** egy ingyenes [Tailscale](https://tailscale.com) fiók és egy WiFi companion node. Az ajánlott [MeshCore Tailscale Companion](https://github.com/petelash/meshcore-tailscale-companion) firmware-rel semmi más nem kell. Más WiFi firmware esetén otthon kell egy mindig bekapcsolt eszköz is, amely Tailscale *subnet routerként* működik (pl. Raspberry Pi, NAS vagy Tailscale-es router), hogy az alkalmazás elérje a node otthoni IP-címét.

## Ajánlott firmware: MeshCore Tailscale Companion
A MeshCore Go és a **[MeshCore Tailscale Companion](https://github.com/petelash/meshcore-tailscale-companion)** ugyanannak a projektnek két része, és együtt működnek a legjobban.

- A firmware a **Seeed Studio XIAO ESP32S3 + Wio-SX1262** eszközön fut, és a **Tailscale VPN közvetlenül a node-ba van beépítve**.
- A node magától csatlakozik a tailnetedhez, és 100.x.x.x címet kap, így **otthon nem kell külön számítógép vagy subnet router** – csak a node, WiFi és áram.
- A MeshCore Go-ban nyisd meg a Tailscale → *Eszközök a tailnetben* menüt, és koppints a node-ra a csatlakozáshoz.
- Egy kattintással telepítheted és frissítheted a **[webes flasherrel](https://petelash.github.io/meshcore-tailscale-companion/)** (Chrome vagy Edge számítógépen).

Ezt a firmware-t ajánljuk a MeshCore Go Tailscale-en keresztüli használatához. Az alkalmazás minden más MeshCore companion firmware-rel is működik.

Ez a tároló csak a **kiadásokat** (APK-fájlokat) tartalmazza. A forráskód nem nyilvános.

## Funkciók
- Csatlakozás WiFi-n (TCP, LAN vagy Tailscale), Bluetooth LE-n vagy USB-n
- Közvetlen üzenetek, csatornák és room serverek; kézbesítési állapot és újrapróbálás (direct / flood)
- Üzenetútvonalak a térképen, a csatornaüzenetedet továbbító átjátszók
- Közvetlen üzenetek útvonalának beállítása (automatikus, mindig flood, kézi útvonal)
- Régió scope (alapértelmezett a node-on és csatornánként)
- Értesítések csatornánként és kontaktonként, fogadott advertek, átjátszók kezelése (állapot, telemetria, CLI)
- Térkép MeshCore node-szimbólumokkal, világos / sötét / AMOLED téma
- Nyelvek: horvát, szerb, angol, német, magyar
- Beépített frissítésellenőrzés

## Letöltés és telepítés
1. Nyisd meg a **[Releases](../../releases/latest)** oldalt, és töltsd le a telefonodnak megfelelő APK-t:
   - `…-arm64.apk` – szinte minden telefon az elmúlt évekből (ajánlott)
   - `…-armv7.apk` – régebbi 32 bites telefonok
   - `…-universal.apk` – ha nem vagy biztos benne (nagyobb)
2. Nyisd meg a fájlt, és ha az Android kéri, engedélyezd az „Ismeretlen alkalmazások telepítése” lehetőséget a böngésződnek vagy fájlkezelődnek.

## Frissítések
Az egyes verziók változásai: **[CHANGELOG](CHANGELOG.md)** (angolul és horvátul).

Az alkalmazás naponta egyszer ellenőrzi ezt a tárolót (Beállítások → Névjegy → *Frissítések keresése*, kikapcsolható). Ha van újabb verzió, felajánlja a letöltését; ezután az Android megerősítést kér a telepítéshez. Az üzeneteid és beállításaid megmaradnak.

## Licenc
MeshCore Go © 2026 Marinko Vrbanić, az **[MIT licenc](LICENSE)** alatt kiadva.
Szabadon használhatod, másolhatod, módosíthatod és megoszthatod, ha megtartod a szerzői jogi megjegyzést és a licenc szövegét.
Az alkalmazás **„ahogy van”, mindenféle garancia nélkül** kerül átadásra; a szerző nem felel a használatából eredő károkért.

Nem hivatalos kliens – nem kapcsolódik a MeshCore projekthez és a Tailscale Inc. céghez. A MeshCore és a Tailscale a tulajdonosaiké.

A nyílt forráskódú komponensek és licenceik a fenti táblázatban (angol rész) és az alkalmazásban találhatók: Beállítások → Névjegy → Licenc.
