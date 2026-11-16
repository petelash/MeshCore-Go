# Changelog / Popis promjena

**English** · [Hrvatski](#hrvatski)

All notable user-facing changes to MeshCore Go, newest first.

## 1.0.1
- **Discover regions in range** – when choosing a region scope (default or per channel), the app asks the repeaters in direct range which regions they serve and lets you pick one with a tap.

## 1.0.0 – first stable release
- Channel icons as in the original MeshCore app: ((•)) for Public, # for hashtag channels, a lock for private channels.

## 0.9.9
- Links in messages are underlined and open in the browser.
- Settings → Radio → **Path hash size** (1, 2 or 3 bytes per hop, stored on the node).
- Radio settings offer **all 48 regional presets**.
- TX power can no longer be set below 1 dBm.
- Notifications show only the MeshCore Go icon.

## 0.9.8
- Fixed the update check.
- Settings → About → **Licence**: MIT licence and the open-source components used.

## 0.9.6
- **In-app updates**: the app checks for new versions once a day and offers download and install (can be turned off).

## 0.9.5
- Contacts whose name ends with an emoji or flag get that emoji as their icon.
- Long-press a contact → **Contact icon**: automatic, 1 letter, 2 letters or any emoji.

## 0.9.1 – 0.9.4
- Each contact category (All, Chat, Repeaters, Chat rooms, Sensors, Favourites) can be sorted: favourites first, latest activity, A–Z or last heard. Long-press the category to change the order; the order is remembered per category.
- "Favourites first" lists favourites and then everyone else alphabetically.
- Better visibility of switches in the AMOLED theme.

## 0.9.0
- **Region scope**: default scope stored on the node and an individual scope per channel (default, no scope or a chosen region).
- **Notification settings**: direct messages, channels, chat rooms, mentions only, link-lost alert, sound and vibration.
- Per channel notifications: all messages, mentions only or muted. Contacts can be muted. Every message notification has a **Mute** button.
- New languages: **Serbian** and **German** (along with Croatian and English).

## 0.8.7
- **AMOLED theme** with the backgrounds of the original MeshCore app.

## 0.8.6
- The repeater `neighbors` command shows names, time and SNR instead of key prefixes.

## 0.8.5
- When a message arrived over several routes, the map shows **all routes at once in different colours**, with a legend.

## 0.8.3 – 0.8.4
- **Path on map** also for your own direct messages and your own channel messages.

## 0.8.2
- Every sent direct message shows how it went out: direct or flood, and which attempt.

## 0.8.1
- Long-press a contact: add to / remove from favourites, rename, delete.

## 0.7.9 – 0.8.0
- More compact lists (contacts, channels, settings, received adverts).

## 0.7.4 – 0.7.8
- **Received adverts** screen (like Discover in the original app): nodes heard by your node, filters by type, details, one-tap add, automatic adding on/off.
- With manual adding on, new adverts are no longer added to contacts automatically.
- "Heard by repeaters" counter under your channel messages.

## 0.7.1 – 0.7.3
- Number of repeaters that heard your channel message, with the list of repeaters and their SNR.
- Long-press a message: reply (@mention), copy, path on map, resend, delete.
- **Message path on the map** (red dashed line with direction arrows).
- **DM route control**: automatic, always flood or a manual path through chosen repeaters.
- Unread messages button that takes you straight to the newest unread conversation.

## 0.7.0 and earlier
- Connection over WiFi (LAN or **built-in Tailscale VPN**, switching automatically), Bluetooth LE and USB.
- Direct messages, channels, room servers, repeater administration (login, status, telemetry, CLI).
- Map with MeshCore node symbols coloured by age.
- Background operation with automatic reconnect.
- Croatian and English, light and dark theme.

---

<a id="hrvatski"></a>
# Popis promjena (hrvatski)

Sve važnije promjene u MeshCore Go za korisnike, od najnovije.

## 1.0.1
- **Otkrij regije u dometu** – pri odabiru scopea regije (zadanog ili za kanal) aplikacija pita repetitore u izravnom dometu koje regije poslužuju, a regiju odabireš jednim dodirom.

## 1.0.0 – prva stabilna verzija
- Ikone kanala kao u originalnoj MeshCore aplikaciji: ((•)) za Public, # za hashtag kanale, lokot za privatne kanale.

## 0.9.9
- Linkovi u porukama su podcrtani i otvaraju se u pregledniku.
- Postavke → Radio → **Veličina hasha putanje** (1, 2 ili 3 bajta po hopu, sprema se na node).
- U radio postavkama dostupno je **svih 48 regionalnih preseta**.
- TX snaga se više ne može postaviti ispod 1 dBm.
- Obavijesti prikazuju samo ikonu MeshCore Go.

## 0.9.8
- Ispravljena provjera ažuriranja.
- Postavke → O aplikaciji → **Licenca**: MIT licenca i korištene komponente otvorenog koda.

## 0.9.6
- **Ažuriranje kroz aplikaciju**: aplikacija jednom dnevno provjerava ima li nova verzija i nudi preuzimanje i instalaciju (može se isključiti).

## 0.9.5
- Kontakti čije ime završava emojijem ili zastavom dobivaju taj emoji kao ikonu.
- Dugi pritisak na kontakt → **Ikona kontakta**: automatski, 1 slovo, 2 slova ili bilo koji emoji.

## 0.9.1 – 0.9.4
- Svaka kategorija kontakata (Svi, Chat, Repetitori, Chat sobe, Senzori, Favoriti) može se sortirati: prvo favoriti, zadnja aktivnost, abeceda ili zadnje čuti. Redoslijed se mijenja dugim pritiskom na kategoriju i pamti se za svaku posebno.
- "Prvo favoriti" prikazuje favorite, a zatim ostale kontakte, abecedno.
- Bolja vidljivost prekidača u AMOLED temi.

## 0.9.0
- **Scope regije**: zadani scope spremljen na nodeu i zaseban scope za svaki kanal (zadani, bez scopea ili odabrana regija).
- **Postavke obavijesti**: privatne poruke, kanali, chat sobe, samo spominjanja, obavijest o prekidu veze, zvuk i vibracija.
- Obavijesti po kanalu: sve poruke, samo spominjanja ili utišano. Kontakti se mogu utišati. Svaka obavijest o poruci ima gumb **Utišaj**.
- Novi jezici: **srpski** i **njemački** (uz hrvatski i engleski).

## 0.8.7
- **AMOLED tema** s pozadinama kao u originalnoj MeshCore aplikaciji.

## 0.8.6
- Naredba `neighbors` na repetitoru prikazuje imena, vrijeme i SNR umjesto kodova ključeva.

## 0.8.5
- Kad je poruka stigla različitim rutama, karta prikazuje **sve rute odjednom u različitim bojama**, s legendom.

## 0.8.3 – 0.8.4
- **Putanja na karti** i za tvoje privatne poruke i tvoje poruke u kanalima.

## 0.8.2
- Uz svaku poslanu privatnu poruku piše kako je otišla: direktno ili floodom i koji je pokušaj.

## 0.8.1
- Dugi pritisak na kontakt: dodaj u favorite / ukloni iz favorita, preimenuj, obriši.

## 0.7.9 – 0.8.0
- Zbijeniji popisi (kontakti, kanali, postavke, primljeni adverti).

## 0.7.4 – 0.7.8
- Ekran **Primljeni adverti** (kao Discover u originalnoj aplikaciji): nodeovi koje je čuo tvoj node, filteri po vrsti, detalji, dodavanje jednim dodirom, uključivanje i isključivanje automatskog dodavanja.
- Kad je uključeno ručno dodavanje, novi adverti se više ne upisuju sami u kontakte.
- Brojač "Čulo repetitora" ispod tvojih poruka u kanalu.

## 0.7.1 – 0.7.3
- Broj repetitora koji su čuli tvoju poruku u kanalu, s popisom repetitora i njihovim SNR-om.
- Dugi pritisak na poruku: odgovori (@spominjanje), kopiraj, putanja na karti, pošalji ponovno, obriši.
- **Putanja poruke na karti** (crvena isprekidana crta sa strelicama smjera).
- **Kontrola rute za DM**: automatski, uvijek flood ili ručna putanja preko odabranih repetitora.
- Gumb za nepročitane poruke koji vodi ravno u najnoviji nepročitani razgovor.

## 0.7.0 i ranije
- Spajanje preko WiFi-ja (LAN ili **ugrađeni Tailscale VPN**, s automatskim prebacivanjem), Bluetootha LE i USB-a.
- Privatne poruke, kanali, chat sobe, administracija repetitora (prijava, status, telemetrija, CLI).
- Karta sa simbolima MeshCore nodeova obojenima prema starosti.
- Rad u pozadini s automatskim ponovnim spajanjem.
- Hrvatski i engleski, svijetla i tamna tema.
