# MeshCore Go

**English** · [Hrvatski](#hrvatski) · [Srpski](#srpski) · [Deutsch](#deutsch) · [Magyar](#magyar) · [Română](#romana) · [Български](#bulgarski) · [Slovenščina](#slovenscina)

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
- Languages: Croatian, Serbian, English, German, Hungarian, Romanian, Bulgarian, Slovenian
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
- Jezici: hrvatski, srpski, engleski, njemački, mađarski, rumunjski, bugarski, slovenski
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
- Nyelvek: horvát, szerb, angol, német, magyar, román, bolgár, szlovén
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

---

<a id="srpski"></a>
# MeshCore Go (srpski)

Android klijent za [MeshCore](https://meshcore.co.uk) LoRa mesh mreže.

> 🔗 **Povezani projekat:** MeshCore Go je usko povezan sa **[MeshCore Tailscale Companion](https://github.com/petelash/meshcore-tailscale-companion)**, našim companion firmverom sa Tailscale-om ugrađenim u sam nod. Preporučuje se korišćenje tog firmvera sa ovom aplikacijom.

> ### 👉 [Web fleš alat: stavi Tailscale VPN na svoj nod](https://petelash.github.io/meshcore-tailscale-companion/)
> Pomoću **[web fleš alata](https://petelash.github.io/meshcore-tailscale-companion/)** jednim klikom instaliraš MeshCore Tailscale Companion firmver na **Seeed Studio XIAO ESP32S3 + Wio-SX1262** (Chrome ili Edge na računaru, USB kabl).
> Firmver ima **Tailscale VPN ugrađen u sam nod**: nod se sam priključuje tvom privatnom, šifrovanom tailnetu i dobija adresu 100.x.x.x.
> MeshCore Go sa svojim ugrađenim Tailscale-om zatim dolazi do noda **bilo gde preko interneta** (mobilni podaci ili bilo koji WiFi) – bez subnet routera,
> bez Raspberry Pi-ja, bez otvaranja portova i bez javne IP adrese. Ista stranica kasnije ažurira i firmver, uz zadržavanje svih podešavanja.

**MeshCore Go je potpuna MeshCore aplikacija za svakodnevnu upotrebu** – koristiš je isto kao zvaničnu MeshCore aplikaciju: povezuješ companion nod preko **Bluetooth LE, USB-a ili WiFi-ja**, dopisuješ se u kanalima i privatnim porukama, gledaš nodove na mapi, upravljaš repetitorima i chat sobama. **Radi sa svim MeshCore companion nodovima**, bilo da nod nosiš sa sobom ili ti stoji na stolu.

**Uz to ima jednu dodatnu mogućnost**, zbog koje je aplikacija i nastala: **ugrađeni Tailscale VPN**. Sa njim svoj MeshCore nod možeš koristiti sa bilo kog mesta preko interneta, a nod pritom ostaje kod kuće (vidi dole). Ne moraš da ga koristiš – bez Tailscale-a aplikacija radi kao i svaki drugi MeshCore klijent.

## Nod ostaje kod kuće, MeshCore ide sa tobom
Tvoj nod može da ostane kod kuće – na krovu, pored prozora ili gde ima najbolji domet – povezan na WiFi i struju. Zahvaljujući **ugrađenom Tailscale VPN-u**, aplikacija do njega dolazi bilo gde preko interneta (mobilni podaci ili bilo koji WiFi), pa možeš da čitaš i šalješ MeshCore poruke, gledaš mapu i upravljaš nodom **bez nošenja noda sa sobom**.

- Nisu potrebni otvoreni portovi ni javna IP adresa: Tailscale pravi privatnu, šifrovanu vezu između tvog telefona i kućne mreže.
- Kod kuće aplikacija razgovara sa nodom direktno preko WiFi-ja, a van kuće sama prelazi na Tailscale.
- Nod ostaje tamo gde mu antena najbolje radi i prima poruke dok tebe nema.

**Šta je potrebno:** besplatan [Tailscale](https://tailscale.com) nalog i WiFi companion nod. Uz preporučeni firmver [MeshCore Tailscale Companion](https://github.com/petelash/meshcore-tailscale-companion) ništa drugo nije potrebno. Sa drugim WiFi firmverom kod kuće ti treba i uređaj koji je stalno uključen i služi kao Tailscale *subnet router* (npr. Raspberry Pi, NAS ili ruter sa Tailscale-om), da aplikacija dođe do kućne IP adrese noda.

## Preporučeni firmver: MeshCore Tailscale Companion
MeshCore Go i **[MeshCore Tailscale Companion](https://github.com/petelash/meshcore-tailscale-companion)** su dva dela istog projekta i najbolje rade zajedno.

- Firmver radi na **Seeed Studio XIAO ESP32S3 + Wio-SX1262** i ima **Tailscale VPN ugrađen direktno u nod**.
- Nod se sam priključuje tvom tailnetu i dobija adresu 100.x.x.x, pa **kod kuće ne treba dodatni računar ni subnet router** – samo nod, WiFi i struja.
- U MeshCore Go otvori Tailscale → *Uređaji u tailnetu* i dodirni nod da se povežeš.
- Instaliraj i ažuriraj ga jednim klikom u **[web fleš alatu](https://petelash.github.io/meshcore-tailscale-companion/)** (Chrome ili Edge na računaru).

Ovaj firmver preporučujemo za korišćenje MeshCore Go preko Tailscale-a. Aplikacija i dalje radi sa svakim drugim MeshCore companion firmverom.

Ovaj repozitorijum sadrži samo **izdanja** (APK fajlove). Izvorni kod nije javan.

## Mogućnosti
- Povezivanje preko WiFi-ja (TCP, LAN ili Tailscale), Bluetooth LE ili USB-a
- Privatne poruke, kanali i chat sobe; status isporuke i ponovni pokušaji (direktno / flood)
- Putanje poruka na mapi, repetitori koji su prosledili tvoju poruku u kanalu
- Kontrola rute privatnih poruka (automatski, uvek flood, ručna putanja)
- Scope regije (zadani na nodu i po kanalu)
- Obaveštenja po kanalu i po kontaktu, primljeni adverti, administracija repetitora (status, telemetrija, CLI)
- Mapa sa MeshCore simbolima nodova, svetla / tamna / AMOLED tema
- Jezici: hrvatski, srpski, engleski, nemački, mađarski, rumunski, bugarski, slovenački
- Ugrađena provera ažuriranja

## Preuzimanje i instalacija
1. Otvori **[Releases](../../releases/latest)** i preuzmi APK za svoj telefon:
   - `…-arm64.apk` – skoro svi telefoni iz poslednjih godina (preporučeno)
   - `…-armv7.apk` – stariji 32-bitni telefoni
   - `…-universal.apk` – ako nisi siguran (veći)
2. Otvori fajl i dozvoli „Instalaciju nepoznatih aplikacija” svom pregledaču ili menadžeru fajlova kada Android to zatraži.

## Ažuriranja
Šta se promenilo u kojoj verziji: **[CHANGELOG](CHANGELOG.md)** (na engleskom i hrvatskom).

Aplikacija jednom dnevno proverava ovaj repozitorijum (Podešavanja → O aplikaciji → *Proveri ažuriranje*, može da se isključi). Kada postoji novija verzija, nudi da je preuzme; zatim Android traži potvrdu instalacije. Tvoje poruke i podešavanja ostaju.

## Licenca
MeshCore Go © 2026 Marinko Vrbanić, objavljeno pod **[MIT licencom](LICENSE)**.
Aplikaciju smeš slobodno da koristiš, kopiraš, menjaš i deliš, uz uslov da zadržiš navod autora i tekst licence.
Aplikacija se daje **„takva kakva jeste”, bez ikakve garancije**; autor ne odgovara za štetu nastalu njenim korišćenjem.

Nezvanični klijent – nije povezan sa MeshCore projektom ni sa kompanijom Tailscale Inc. MeshCore i Tailscale pripadaju svojim vlasnicima.

Komponente otvorenog koda i njihove licence navedene su u tabeli iznad (engleski deo) i u aplikaciji: Podešavanja → O aplikaciji → Licenca.

---

<a id="deutsch"></a>
# MeshCore Go (Deutsch)

Android-Client für [MeshCore](https://meshcore.co.uk) LoRa-Mesh-Netzwerke.

> 🔗 **Begleitprojekt:** MeshCore Go ist eng mit **[MeshCore Tailscale Companion](https://github.com/petelash/meshcore-tailscale-companion)** verbunden, unserer Companion-Firmware mit im Node eingebautem Tailscale. Diese Firmware wird zusammen mit der App empfohlen.

> ### 👉 [Web-Flasher: Tailscale-VPN auf deinen Node bringen](https://petelash.github.io/meshcore-tailscale-companion/)
> Mit dem **[Web-Flasher](https://petelash.github.io/meshcore-tailscale-companion/)** installierst du die Firmware MeshCore Tailscale Companion mit einem Klick auf einem **Seeed Studio XIAO ESP32S3 + Wio-SX1262** (Chrome oder Edge am Computer, USB-Kabel).
> Die Firmware hat das **Tailscale-VPN direkt im Node eingebaut**: Der Node tritt von selbst deinem privaten, verschlüsselten Tailnet bei und erhält eine 100.x.x.x-Adresse.
> MeshCore Go mit seinem eigenen eingebauten Tailscale erreicht den Node dann **von überall über das Internet** (mobile Daten oder jedes WLAN) – ohne Subnet-Router,
> ohne Raspberry Pi, ohne Portweiterleitung und ohne öffentliche IP-Adresse. Über dieselbe Seite aktualisierst du die Firmware später auch, alle Einstellungen bleiben erhalten.

**MeshCore Go ist eine vollständige MeshCore-App für den Alltag** – du nutzt sie genau wie die offizielle MeshCore-App: Verbinde deinen Companion-Node per **Bluetooth LE, USB oder WLAN**, chatte in Kanälen und Direktnachrichten, sieh Nodes auf der Karte, verwalte Repeater und Chaträume. Sie **funktioniert mit jedem MeshCore-Companion-Node**, egal ob du ihn bei dir trägst oder auf dem Schreibtisch hast.

**Dazu hat sie eine zusätzliche Funktion**, für die die App entstanden ist: ein **eingebautes Tailscale-VPN**. Damit kannst du deinen MeshCore-Node von überall über das Internet nutzen, während der Node selbst zu Hause bleibt (siehe unten). Du musst es nicht nutzen – ohne Tailscale funktioniert die App wie jeder andere MeshCore-Client.

## Den Node zu Hause lassen, MeshCore mitnehmen
Dein Node kann zu Hause bleiben – auf dem Dach, am Fenster oder wo er den besten Empfang hat –, mit WLAN und Strom verbunden. Dank des **eingebauten Tailscale-VPNs** erreicht ihn die App von überall über das Internet (mobile Daten oder jedes WLAN), sodass du MeshCore-Nachrichten lesen und senden, die Karte ansehen und den Node verwalten kannst, **ohne den Node mitzunehmen**.

- Keine Portweiterleitung und keine öffentliche IP nötig: Tailscale stellt eine private, verschlüsselte Verbindung zwischen deinem Handy und deinem Heimnetz her.
- Zu Hause spricht die App direkt über WLAN mit dem Node, unterwegs wechselt sie von selbst zu Tailscale.
- Der Node bleibt dort, wo seine Antenne am besten funktioniert, und empfängt weiter Nachrichten, während du weg bist.

**Was du brauchst:** ein kostenloses [Tailscale](https://tailscale.com)-Konto und einen WLAN-Companion-Node. Mit der empfohlenen Firmware [MeshCore Tailscale Companion](https://github.com/petelash/meshcore-tailscale-companion) brauchst du nichts weiter. Bei anderer WLAN-Firmware brauchst du zu Hause zusätzlich ein dauerhaft eingeschaltetes Gerät, das als Tailscale-*Subnet-Router* dient (z. B. Raspberry Pi, NAS oder ein Router mit Tailscale), damit die App die Heim-IP-Adresse des Nodes erreicht.

## Empfohlene Firmware: MeshCore Tailscale Companion
MeshCore Go und **[MeshCore Tailscale Companion](https://github.com/petelash/meshcore-tailscale-companion)** sind zwei Teile desselben Projekts und funktionieren zusammen am besten.

- Die Firmware läuft auf dem **Seeed Studio XIAO ESP32S3 + Wio-SX1262** und hat das **Tailscale-VPN direkt im Node eingebaut**.
- Der Node tritt von selbst deinem Tailnet bei und erhält eine 100.x.x.x-Adresse, daher **braucht es zu Hause keinen zusätzlichen Computer und keinen Subnet-Router** – nur Node, WLAN und Strom.
- Öffne in MeshCore Go Tailscale → *Geräte im Tailnet* und tippe auf den Node, um dich zu verbinden.
- Installiere und aktualisiere sie mit einem Klick im **[Web-Flasher](https://petelash.github.io/meshcore-tailscale-companion/)** (Chrome oder Edge am Computer).

Wir empfehlen diese Firmware, um MeshCore Go über Tailscale zu nutzen. Die App funktioniert weiterhin mit jeder anderen MeshCore-Companion-Firmware.

Dieses Repository enthält nur die **Releases** (APK-Dateien). Der Quellcode ist nicht öffentlich.

## Funktionen
- Verbindung per WLAN (TCP, LAN oder Tailscale), Bluetooth LE oder USB
- Direktnachrichten, Kanäle und Chaträume; Zustellstatus und Wiederholungen (direkt / Flood)
- Nachrichtenrouten auf der Karte, Repeater, die deine Kanalnachricht weitergeleitet haben
- Routensteuerung für Direktnachrichten (automatisch, immer Flood, manueller Pfad)
- Regions-Scope (Standard am Node und pro Kanal)
- Benachrichtigungen pro Kanal und pro Kontakt, empfangene Adverts, Repeater-Administration (Status, Telemetrie, CLI)
- Karte mit MeshCore-Node-Symbolen, helles / dunkles / AMOLED-Design
- Sprachen: Kroatisch, Serbisch, Englisch, Deutsch, Ungarisch, Rumänisch, Bulgarisch, Slowenisch
- Integrierte Update-Prüfung

## Download und Installation
1. Öffne **[Releases](../../releases/latest)** und lade die APK für dein Handy herunter:
   - `…-arm64.apk` – fast alle Handys der letzten Jahre (empfohlen)
   - `…-armv7.apk` – ältere 32-Bit-Handys
   - `…-universal.apk` – wenn du unsicher bist (größer)
2. Öffne die Datei und erlaube „Installation unbekannter Apps” für deinen Browser oder Dateimanager, wenn Android danach fragt.

## Updates
Was sich in welcher Version geändert hat: **[CHANGELOG](CHANGELOG.md)** (auf Englisch und Kroatisch).

Die App prüft dieses Repository einmal täglich (Einstellungen → Über die App → *Nach Updates suchen*, abschaltbar). Gibt es eine neuere Version, bietet sie den Download an; danach bittet Android um die Bestätigung der Installation. Deine Nachrichten und Einstellungen bleiben erhalten.

## Lizenz
MeshCore Go © 2026 Marinko Vrbanić, veröffentlicht unter der **[MIT-Lizenz](LICENSE)**.
Du darfst die App frei nutzen, kopieren, verändern und weitergeben, solange du den Urhebervermerk und den Lizenztext beibehältst.
Die App wird **„wie besehen”, ohne jegliche Gewährleistung** bereitgestellt; der Autor haftet nicht für Schäden, die aus ihrer Nutzung entstehen.

Inoffizieller Client – nicht mit dem MeshCore-Projekt oder Tailscale Inc. verbunden. MeshCore und Tailscale gehören ihren Eigentümern.

Die Open-Source-Komponenten und ihre Lizenzen stehen in der Tabelle oben (englischer Teil) und in der App: Einstellungen → Über die App → Lizenz.

---

<a id="romana"></a>
# MeshCore Go (română)

Client Android pentru rețelele mesh LoRa [MeshCore](https://meshcore.co.uk).

> 🔗 **Proiect asociat:** MeshCore Go este strâns legat de **[MeshCore Tailscale Companion](https://github.com/petelash/meshcore-tailscale-companion)**, firmware-ul nostru companion cu Tailscale integrat chiar în nod. Utilizarea acestui firmware împreună cu aplicația este recomandată.

> ### 👉 [Web flasher: pune Tailscale VPN pe nodul tău](https://petelash.github.io/meshcore-tailscale-companion/)
> Cu **[web flasher-ul](https://petelash.github.io/meshcore-tailscale-companion/)** instalezi firmware-ul MeshCore Tailscale Companion pe un **Seeed Studio XIAO ESP32S3 + Wio-SX1262** cu un singur clic (Chrome sau Edge pe un computer, cablu USB).
> Firmware-ul are **Tailscale VPN integrat în nod**: nodul se alătură singur tailnet-ului tău privat și criptat și primește o adresă 100.x.x.x.
> MeshCore Go, cu propriul Tailscale integrat, ajunge apoi la nod **de oriunde prin internet** (date mobile sau orice WiFi) – fără subnet router,
> fără Raspberry Pi, fără redirecționare de porturi și fără adresă IP publică. Aceeași pagină actualizează ulterior și firmware-ul, păstrând toate setările.

**MeshCore Go este o aplicație MeshCore completă, pentru fiecare zi** – o folosești exact ca aplicația oficială MeshCore: conectezi nodul companion prin **Bluetooth LE, USB sau WiFi**, scrii în canale și în mesaje private, vezi nodurile pe hartă, gestionezi repetoare și camere de chat. **Funcționează cu orice nod MeshCore companion**, fie că îl porți cu tine, fie că stă pe birou.

**În plus are o funcție extra**, motivul pentru care a fost creată aplicația: un **Tailscale VPN integrat**. Cu el îți poți folosi nodul MeshCore de oriunde prin internet, în timp ce nodul rămâne acasă (vezi mai jos). Nu ești obligat să-l folosești – fără Tailscale aplicația funcționează ca orice alt client MeshCore.

## Nodul rămâne acasă, MeshCore merge cu tine
Nodul tău poate rămâne acasă – pe acoperiș, lângă fereastră sau unde are cea mai bună acoperire – conectat la WiFi și la curent. Datorită **Tailscale VPN-ului integrat**, aplicația ajunge la el de oriunde prin internet (date mobile sau orice WiFi), așa că poți citi și trimite mesaje MeshCore, vedea harta și gestiona nodul **fără să-l porți cu tine**.

- Nu ai nevoie de redirecționare de porturi sau de IP public: Tailscale creează o conexiune privată și criptată între telefon și rețeaua ta de acasă.
- Acasă aplicația vorbește direct cu nodul prin WiFi; în afara casei trece singură pe Tailscale.
- Nodul rămâne acolo unde antena lui funcționează cel mai bine și continuă să primească mesaje cât timp ești plecat.

**Ce îți trebuie:** un cont [Tailscale](https://tailscale.com) gratuit și un nod companion WiFi. Cu firmware-ul recomandat [MeshCore Tailscale Companion](https://github.com/petelash/meshcore-tailscale-companion) nu mai trebuie nimic altceva. Cu alt firmware WiFi îți trebuie acasă și un dispozitiv mereu pornit care funcționează ca *subnet router* Tailscale (de ex. un Raspberry Pi, un NAS sau un router cu Tailscale), ca aplicația să ajungă la adresa IP de acasă a nodului.

## Firmware recomandat: MeshCore Tailscale Companion
MeshCore Go și **[MeshCore Tailscale Companion](https://github.com/petelash/meshcore-tailscale-companion)** sunt două părți ale aceluiași proiect și funcționează cel mai bine împreună.

- Firmware-ul rulează pe **Seeed Studio XIAO ESP32S3 + Wio-SX1262** și are **Tailscale VPN integrat direct în nod**.
- Nodul se alătură singur tailnet-ului tău și primește o adresă 100.x.x.x, deci **nu ai nevoie acasă de un computer suplimentar sau de un subnet router** – doar de nod, WiFi și curent.
- În MeshCore Go deschide Tailscale → *Dispozitive în tailnet* și atinge nodul pentru a te conecta.
- Îl instalezi și îl actualizezi cu un singur clic în **[web flasher](https://petelash.github.io/meshcore-tailscale-companion/)** (Chrome sau Edge pe un computer).

Recomandăm acest firmware pentru utilizarea MeshCore Go prin Tailscale. Aplicația funcționează în continuare cu orice alt firmware MeshCore companion.

Acest depozit conține doar **versiunile** (fișiere APK). Codul sursă nu este public.

## Funcții
- Conectare prin WiFi (TCP, LAN sau Tailscale), Bluetooth LE sau USB
- Mesaje private, canale și camere de chat; stare de livrare și reîncercări (direct / flood)
- Traseele mesajelor pe hartă, repetoare care au retransmis mesajul tău pe canal
- Controlul rutei mesajelor private (automat, mereu flood, traseu manual)
- Scope de regiune (implicit pe nod și pe canal)
- Notificări pe canal și pe contact, advert-uri primite, administrarea repetoarelor (stare, telemetrie, CLI)
- Hartă cu simboluri MeshCore pentru noduri, temă luminoasă / întunecată / AMOLED
- Limbi: croată, sârbă, engleză, germană, maghiară, română, bulgară, slovenă
- Verificare de actualizări integrată

## Descărcare și instalare
1. Deschide **[Releases](../../releases/latest)** și descarcă APK-ul potrivit telefonului tău:
   - `…-arm64.apk` – aproape toate telefoanele din ultimii ani (recomandat)
   - `…-armv7.apk` – telefoane mai vechi pe 32 de biți
   - `…-universal.apk` – dacă nu ești sigur (mai mare)
2. Deschide fișierul și permite „Instalarea aplicațiilor necunoscute” pentru browser sau managerul de fișiere, când Android îți cere.

## Actualizări
Ce s-a schimbat în fiecare versiune: **[CHANGELOG](CHANGELOG.md)** (în engleză și croată).

Aplicația verifică acest depozit o dată pe zi (Setări → Despre aplicație → *Caută actualizări*, poate fi oprit). Când există o versiune mai nouă, oferă să o descarce; apoi Android cere confirmarea instalării. Mesajele și setările tale rămân.

## Licență
MeshCore Go © 2026 Marinko Vrbanić, publicat sub **[licența MIT](LICENSE)**.
Poți folosi, copia, modifica și distribui liber aplicația, cu condiția să păstrezi mențiunea autorului și textul licenței.
Aplicația este oferită **„ca atare”, fără nicio garanție**; autorul nu răspunde pentru daunele rezultate din utilizarea ei.

Client neoficial – nu este afiliat cu proiectul MeshCore sau cu Tailscale Inc. MeshCore și Tailscale aparțin proprietarilor lor.

Componentele open-source și licențele lor sunt listate în tabelul de mai sus (partea în engleză) și în aplicație: Setări → Despre aplicație → Licență.

---

<a id="bulgarski"></a>
# MeshCore Go (български)

Android клиент за [MeshCore](https://meshcore.co.uk) LoRa mesh мрежи.

> 🔗 **Свързан проект:** MeshCore Go е тясно свързан с **[MeshCore Tailscale Companion](https://github.com/petelash/meshcore-tailscale-companion)** – нашия companion firmware с Tailscale, вграден в самия възел. Препоръчва се използването на този firmware с приложението.

> ### 👉 [Web flasher: сложи Tailscale VPN на своя възел](https://petelash.github.io/meshcore-tailscale-companion/)
> С **[web flasher](https://petelash.github.io/meshcore-tailscale-companion/)** инсталираш firmware-а MeshCore Tailscale Companion на **Seeed Studio XIAO ESP32S3 + Wio-SX1262** с едно кликване (Chrome или Edge на компютър, USB кабел).
> Firmware-ът има **Tailscale VPN, вграден във възела**: възелът сам се присъединява към твоя частен, шифрован tailnet и получава адрес 100.x.x.x.
> MeshCore Go със собствения си вграден Tailscale достига възела **отвсякъде през интернет** (мобилни данни или всякакъв WiFi) – без subnet router,
> без Raspberry Pi, без пренасочване на портове и без публичен IP адрес. Същата страница по-късно обновява и firmware-а, като запазва всички настройки.

**MeshCore Go е пълноценно MeshCore приложение за всеки ден** – ползваш го точно както официалното MeshCore приложение: свързваш companion възела си през **Bluetooth LE, USB или WiFi**, пишеш в канали и лични съобщения, виждаш възлите на картата, управляваш репитери и чат стаи. **Работи с всеки MeshCore companion възел**, независимо дали го носиш със себе си, или стои на бюрото ти.

**Освен това има една допълнителна възможност**, заради която е създадено приложението: **вграден Tailscale VPN**. С него можеш да ползваш своя MeshCore възел отвсякъде през интернет, докато самият възел остава вкъщи (виж по-долу). Не е задължително да го ползваш – без Tailscale приложението работи като всеки друг MeshCore клиент.

## Възелът остава вкъщи, MeshCore идва с теб
Твоят възел може да остане вкъщи – на покрива, до прозореца или където има най-добро покритие – свързан към WiFi и захранване. Благодарение на **вградения Tailscale VPN** приложението го достига отвсякъде през интернет (мобилни данни или всякакъв WiFi), така че можеш да четеш и пращаш MeshCore съобщения, да гледаш картата и да управляваш възела **без да го носиш със себе си**.

- Не са нужни пренасочване на портове и публичен IP: Tailscale създава частна, шифрована връзка между телефона ти и домашната ти мрежа.
- Вкъщи приложението говори с възела директно през WiFi, а извън къщи само превключва на Tailscale.
- Възелът остава там, където антената му работи най-добре, и продължава да приема съобщения, докато те няма.

**Какво ти трябва:** безплатен акаунт в [Tailscale](https://tailscale.com) и WiFi companion възел. С препоръчания firmware [MeshCore Tailscale Companion](https://github.com/petelash/meshcore-tailscale-companion) не ти трябва нищо друго. С друг WiFi firmware вкъщи ти трябва и устройство, което е постоянно включено и служи като Tailscale *subnet router* (напр. Raspberry Pi, NAS или рутер с Tailscale), за да достигне приложението домашния IP адрес на възела.

## Препоръчан firmware: MeshCore Tailscale Companion
MeshCore Go и **[MeshCore Tailscale Companion](https://github.com/petelash/meshcore-tailscale-companion)** са две части на един и същ проект и работят най-добре заедно.

- Firmware-ът работи на **Seeed Studio XIAO ESP32S3 + Wio-SX1262** и има **Tailscale VPN, вграден директно във възела**.
- Възелът сам се присъединява към твоя tailnet и получава адрес 100.x.x.x, така че **вкъщи не ти трябва допълнителен компютър или subnet router** – само възелът, WiFi и захранване.
- В MeshCore Go отвори Tailscale → *Устройства в tailnet* и докосни възела, за да се свържеш.
- Инсталирай и обновявай с едно кликване в **[web flasher](https://petelash.github.io/meshcore-tailscale-companion/)** (Chrome или Edge на компютър).

Препоръчваме този firmware за използване на MeshCore Go през Tailscale. Приложението продължава да работи с всеки друг MeshCore companion firmware.

Това хранилище съдържа само **изданията** (APK файлове). Изходният код не е публичен.

## Възможности
- Връзка през WiFi (TCP, LAN или Tailscale), Bluetooth LE или USB
- Лични съобщения, канали и чат стаи; състояние на доставката и повторни опити (direct / flood)
- Пътища на съобщенията на картата, репитери, препратили твоето съобщение в канал
- Управление на маршрута на личните съобщения (автоматично, винаги flood, ръчен път)
- Scope на региона (по подразбиране във възела и за всеки канал)
- Известия за всеки канал и за всеки контакт, получени адверти, администриране на репитери (състояние, телеметрия, CLI)
- Карта със символи на MeshCore възли, светла / тъмна / AMOLED тема
- Езици: хърватски, сръбски, английски, немски, унгарски, румънски, български, словенски
- Вградена проверка за актуализации

## Изтегляне и инсталиране
1. Отвори **[Releases](../../releases/latest)** и изтегли APK за твоя телефон:
   - `…-arm64.apk` – почти всички телефони от последните години (препоръчително)
   - `…-armv7.apk` – по-стари 32-битови телефони
   - `…-universal.apk` – ако не си сигурен (по-голям)
2. Отвори файла и разреши „Инсталиране на неизвестни приложения“ за браузъра или файловия мениджър, когато Android поиска.

## Актуализации
Какво се е променило във всяка версия: **[CHANGELOG](CHANGELOG.md)** (на английски и хърватски).

Приложението проверява това хранилище веднъж дневно (Настройки → За приложението → *Провери за актуализации*, може да се изключи). Когато има по-нова версия, предлага да я изтегли; след това Android иска потвърждение за инсталиране. Съобщенията и настройките ти остават.

## Лиценз
MeshCore Go © 2026 Marinko Vrbanić, публикувано под **[лиценз MIT](LICENSE)**.
Можеш свободно да ползваш, копираш, променяш и споделяш приложението, при условие че запазиш името на автора и текста на лиценза.
Приложението се предоставя **„както е“, без каквато и да е гаранция**; авторът не носи отговорност за вреди от използването му.

Неофициален клиент – не е свързан с проекта MeshCore, нито с Tailscale Inc. MeshCore и Tailscale принадлежат на своите собственици.

Компонентите с отворен код и техните лицензи са изброени в таблицата по-горе (английската част) и в приложението: Настройки → За приложението → Лиценз.

---

<a id="slovenscina"></a>
# MeshCore Go (slovenščina)

Odjemalec za Android za LoRa mesh omrežja [MeshCore](https://meshcore.co.uk).

> 🔗 **Povezan projekt:** MeshCore Go je tesno povezan z **[MeshCore Tailscale Companion](https://github.com/petelash/meshcore-tailscale-companion)**, našo companion programsko opremo (firmware) s Tailscale, vgrajenim v samo vozlišče. Uporaba te programske opreme z aplikacijo je priporočena.

> ### 👉 [Spletni flasher: daj Tailscale VPN na svoje vozlišče](https://petelash.github.io/meshcore-tailscale-companion/)
> S **[spletnim flasherjem](https://petelash.github.io/meshcore-tailscale-companion/)** z enim klikom namestiš firmware MeshCore Tailscale Companion na **Seeed Studio XIAO ESP32S3 + Wio-SX1262** (Chrome ali Edge na računalniku, kabel USB).
> Firmware ima **Tailscale VPN vgrajen v vozlišče**: vozlišče se samo pridruži tvojemu zasebnemu, šifriranemu tailnetu in dobi naslov 100.x.x.x.
> MeshCore Go z lastnim vgrajenim Tailscale nato doseže vozlišče **od koderkoli prek interneta** (mobilni podatki ali kateri koli WiFi) – brez subnet routerja,
> brez Raspberry Pi, brez preusmerjanja vrat in brez javnega IP naslova. Ista stran pozneje posodobi tudi firmware, vse nastavitve ostanejo.

**MeshCore Go je popolna vsakodnevna aplikacija MeshCore** – uporabljaš jo povsem enako kot uradno aplikacijo MeshCore: povežeš companion vozlišče prek **Bluetooth LE, USB ali WiFi**, klepetaš v kanalih in zasebnih sporočilih, gledaš vozlišča na zemljevidu, upravljaš repetitorje in klepetalnice. **Deluje z vsakim MeshCore companion vozliščem**, ne glede na to, ali ga nosiš s seboj ali stoji na mizi.

**Poleg tega ima eno dodatno možnost**, zaradi katere je aplikacija nastala: **vgrajen Tailscale VPN**. Z njim lahko svoje vozlišče MeshCore uporabljaš od koderkoli prek interneta, vozlišče pa medtem ostane doma (glej spodaj). Ni ga treba uporabljati – brez Tailscale aplikacija deluje kot vsak drug odjemalec MeshCore.

## Vozlišče ostane doma, MeshCore gre s tabo
Tvoje vozlišče lahko ostane doma – na strehi, ob oknu ali kjer ima najboljši doseg – povezano na WiFi in napajanje. Zahvaljujoč **vgrajenemu Tailscale VPN** ga aplikacija doseže od koderkoli prek interneta (mobilni podatki ali kateri koli WiFi), zato lahko bereš in pošiljaš sporočila MeshCore, gledaš zemljevid in upravljaš vozlišče **brez nošenja vozlišča s seboj**.

- Ne potrebuješ preusmerjanja vrat ali javnega IP naslova: Tailscale ustvari zasebno, šifrirano povezavo med telefonom in domačim omrežjem.
- Doma aplikacija z vozliščem govori neposredno prek WiFi, zunaj doma pa sama preklopi na Tailscale.
- Vozlišče ostane tam, kjer njegova antena deluje najbolje, in še naprej prejema sporočila, medtem ko te ni.

**Kaj potrebuješ:** brezplačen račun [Tailscale](https://tailscale.com) in WiFi companion vozlišče. S priporočenim firmwareom [MeshCore Tailscale Companion](https://github.com/petelash/meshcore-tailscale-companion) ne potrebuješ ničesar drugega. Pri drugem WiFi firmwareu potrebuješ doma še napravo, ki je vedno vklopljena in služi kot Tailscale *subnet router* (npr. Raspberry Pi, NAS ali usmerjevalnik s Tailscale), da aplikacija doseže domači IP naslov vozlišča.

## Priporočeni firmware: MeshCore Tailscale Companion
MeshCore Go in **[MeshCore Tailscale Companion](https://github.com/petelash/meshcore-tailscale-companion)** sta dela istega projekta in najbolje delujeta skupaj.

- Firmware deluje na **Seeed Studio XIAO ESP32S3 + Wio-SX1262** in ima **Tailscale VPN vgrajen neposredno v vozlišče**.
- Vozlišče se samo pridruži tvojemu tailnetu in dobi naslov 100.x.x.x, zato **doma ne potrebuješ dodatnega računalnika ali subnet routerja** – samo vozlišče, WiFi in napajanje.
- V MeshCore Go odpri Tailscale → *Naprave v tailnetu* in tapni vozlišče za povezavo.
- Namesti in posodabljaj ga z enim klikom v **[spletnem flasherju](https://petelash.github.io/meshcore-tailscale-companion/)** (Chrome ali Edge na računalniku).

Ta firmware priporočamo za uporabo MeshCore Go prek Tailscale. Aplikacija še vedno deluje z vsakim drugim MeshCore companion firmwareom.

Ta repozitorij vsebuje samo **izdaje** (datoteke APK). Izvorna koda ni javna.

## Funkcije
- Povezava prek WiFi (TCP, LAN ali Tailscale), Bluetooth LE ali USB
- Zasebna sporočila, kanali in klepetalnice; stanje dostave in ponovni poskusi (neposredno / flood)
- Poti sporočil na zemljevidu, repetitorji, ki so posredovali tvoje sporočilo v kanalu
- Nadzor poti zasebnih sporočil (samodejno, vedno flood, ročna pot)
- Scope regije (privzeto na vozlišču in za vsak kanal)
- Obvestila za vsak kanal in stik, prejeti adverti, upravljanje repetitorjev (stanje, telemetrija, CLI)
- Zemljevid s simboli vozlišč MeshCore, svetla / temna / AMOLED tema
- Jeziki: hrvaščina, srbščina, angleščina, nemščina, madžarščina, romunščina, bolgarščina, slovenščina
- Vgrajeno preverjanje posodobitev

## Prenos in namestitev
1. Odpri **[Releases](../../releases/latest)** in prenesi APK za svoj telefon:
   - `…-arm64.apk` – skoraj vsi telefoni zadnjih let (priporočeno)
   - `…-armv7.apk` – starejši 32-bitni telefoni
   - `…-universal.apk` – če nisi prepričan (večji)
2. Odpri datoteko in dovoli »Namestitev neznanih aplikacij« svojemu brskalniku ali upravljalniku datotek, ko Android to zahteva.

## Posodobitve
Kaj se je spremenilo v posamezni različici: **[CHANGELOG](CHANGELOG.md)** (v angleščini in hrvaščini).

Aplikacija enkrat na dan preveri ta repozitorij (Nastavitve → O aplikaciji → *Preveri posodobitve*, lahko izklopiš). Ko obstaja novejša različica, ponudi prenos; nato Android zahteva potrditev namestitve. Tvoja sporočila in nastavitve ostanejo.

## Licenca
MeshCore Go © 2026 Marinko Vrbanić, objavljeno pod **[licenco MIT](LICENSE)**.
Aplikacijo smeš prosto uporabljati, kopirati, spreminjati in deliti, če ohraniš navedbo avtorja in besedilo licence.
Aplikacija je ponujena **»takšna, kot je«, brez kakršnega koli jamstva**; avtor ne odgovarja za škodo, nastalo z njeno uporabo.

Neuradni odjemalec – ni povezan s projektom MeshCore ali podjetjem Tailscale Inc. MeshCore in Tailscale pripadata svojima lastnikoma.

Komponente odprte kode in njihove licence so navedene v zgornji tabeli (angleški del) in v aplikaciji: Nastavitve → O aplikaciji → Licenca.
