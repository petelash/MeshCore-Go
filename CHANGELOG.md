# Changelog / Popis promjena

**English** · [Hrvatski](#hrvatski)

All notable user-facing changes to MeshCore Go, newest first.

## 1.1.2
- **Unread messages**: when you open a chat with unread messages, it opens at the first unread one, marked by a line with "Unread messages". Scroll down to the newer ones yourself; a new message moves the list down only when you are already at the bottom.
- "Proslijedilo repetitora" (repeaters that forwarded your message): the number is red while no repeater has forwarded the message and green from one up.

## 1.1.1
- **Channel order**: hold a channel in the Channels tab and drag it up or down to change the order. Holding without moving still opens the channel menu, which now also has **Restore original order**.
- The order is changed and saved **only in the app**, separately for each node, and stays after reconnecting and restarting the app. Nothing is written to the node: the channels keep their slots on the node, and other apps connected to the same node keep their own order.
- **Bluetooth search** shows two lists: **In range** (nodes found by the scan, strongest signal first, with signal bars and dBm, marked *saved* or *new*) and **Saved – not in range** (paired or saved nodes the scan did not find, greyed out but still tappable). The search starts by itself when the Bluetooth tab opens, and saved Bluetooth nodes are no longer listed twice. The signal shown is smoothed (median of the last readings), so the bars no longer flicker, and Bluetooth nodes paired only in Android can also be removed from the list (with a shortcut to the Bluetooth settings to unpair them).
- Saved nodes (WiFi, Tailscale, USB and Bluetooth) no longer have a delete icon: hold a node to remove it, and the app asks for confirmation first.
- Fixed: removing a node the app was still connecting to did not stop the attempts, and Cancel right after start-up could be undone by the background service starting the connection again.
- Fixed: "Proslijedilo repetitora" (repeaters that forwarded your message) stayed at 0 on a channel that exists in more than one slot with the same key, e.g. a second "Public" used with a scope.
- Croatian and Serbian wording: "heard" (čuti) is replaced everywhere, e.g. "Zadnje detektirani", "Detektirani kanali koje nemaš", "Detektiran je kanal …", "Proslijedilo repetitora: N" and "Tvoj signal kod repetitora".

## 1.1.0
- **Hungarian** language (Settings → Appearance → Language → Magyar).
- **Heard #channels you don't have**: the app recognises traffic on #channels that are not added (a built-in list of common channel, city and region names, your own names and channels mentioned in messages) and notifies once per channel, with **Add** and **Don't notify again** buttons. The same channels are listed at the top of the Channels tab, so you add only the ones you want.
- Settings → Notifications: turn these notifications on or off, add your own channel names to watch, and reset the channels you silenced.
- Settings → About: a **Changelog** link under the app version opens the changes of that version.
- Adding and removing a channel is now instant (the app no longer re-reads every channel slot from the node).
- Icon descriptions read by screen readers now follow the selected language.
- Fixed: the sensor contact type was shown as "Sensor" in Croatian and Serbian.

## 1.0.9
- Neighbour repeaters: signal status for each repeater – quality (excellent / good / weak / very weak) with SNR and RSSI, how well the repeater hears you, distance, and average / lowest / highest SNR.
- Neighbour repeaters: sort by last heard, strongest signal or nearest.
- Neighbour repeaters that are not contacts yet can be added with one tap (or all at once); the app first asks the repeater for its full name.
- A short (1-byte) code is merged with the repeater already identified by a longer code; when it still fits several repeaters, tapping the question mark explains which ones, nearest first.

## 1.0.8
- New **Neighbour repeaters** screen in the ⋮ menu (below Received adverts): the repeaters your node hears directly, with full names when known, SNR, RSSI, when each was last heard and how many packets came through it. The refresh button asks the repeaters in range to answer.

## 1.0.7
- Send advert button: a short press sends a zero-hop advert, a long press sends a flood advert.
- Tailscale → Devices in the tailnet: tap a device to connect to the MeshCore node on it (asks for confirmation first; the TCP port can be changed, default 5000).

## 1.0.6
- The number of new received adverts is shown only next to "Received adverts" in the ⋮ menu, no longer on the menu icon.

## 1.0.5
- Fixed notifications: the background connection service now always starts, so messages and notifications keep arriving after you leave the app.
- A chat left open in the background now notifies about new messages and keeps them unread until you return.
- Settings → Notifications warns when Android has notifications turned off for the app, with a shortcut to turn them on.

## 1.0.4
- Send advert button uses the ((•)) symbol, like the original app.
- Contact search opens from the top bar (magnifier icon) instead of a permanent search field.
- Received adverts moved to the ⋮ menu, with a counter of new nodes.

## 1.0.3
- The connection notification shows the node's battery and, over Bluetooth, the signal strength (over WiFi: LAN or Tailscale) instead of the Bluetooth address.
- The connection notification no longer adds an unread badge to the app icon.

## 1.0.2
- The search field looks like the category buttons below it (same outline and rounded corners, compact height) and has a clear button.

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
- **Unread** button: shows how many conversations have unread messages and takes you straight to the newest one.
- Message path on the map drawn as a red dashed line with direction arrows.
- Layout fixes for Android 15 (no empty gaps above lists).

## 0.7.0
- Number of repeaters that heard your channel message, with the list of repeaters and their SNR.
- Long-press a message: reply (@mention), copy, path on map, resend, delete.
- **Message path on the map**: the repeaters a message travelled through.
- **DM route control**: automatic, always flood or a manual path through chosen repeaters.

## 0.6.0
- **Remember password** option for repeater and room server login (stored only on the phone).
- Notifications use the app icon.

## 0.5.0
- Official MeshCore node symbols on the map, coloured by how recently the node was heard.

## 0.4.0
- New app icon.
- **English** language (switch in Settings, along with Croatian).
- Author information in Settings → About.

## 0.3.0
- **Automatic connection route**: at home the app connects directly over WiFi, away from home through Tailscale – nothing to switch manually.
- Simple, round node symbols on the map.

## 0.2.0
- The app is now called **MeshCore Go**.
- Connect to nodes **over the local network without Tailscale, over Bluetooth LE and over USB**.
- Separate map symbols for companions, repeaters, room servers and sensors.
- Adjustable **font size** and choice of fonts.
- **Always running in the background**: ignores battery optimisation, keeps the link to the node and **reconnects automatically** (each can be turned on or off).

## 0.1.0 – first version
- Android MeshCore client with **Tailscale built in**: no separate Tailscale app or system VPN is needed. Sign in with a Tailscale auth key or through the browser.
- Connection to a WiFi companion node over TCP, through your tailnet.
- Contacts, channels and direct messages with delivery receipts; room servers.
- Repeater administration: login, status, trace and CLI console.
- Map of nodes.
- Layout and flow like the original MeshCore app (Contacts, Channels, Map, Settings), in its own design.

---

<a id="hrvatski"></a>
# Popis promjena (hrvatski)

Sve važnije promjene u MeshCore Go za korisnike, od najnovije.

## 1.1.2
- **Nepročitane poruke**: razgovor s nepročitanim porukama otvara se na prvoj nepročitanoj, označenoj crtom s natpisom „Nepročitane poruke”. Prema novijim porukama listaš sam; nova poruka pomiče popis prema dolje samo ako si već na dnu.
- „Proslijedilo repetitora”: broj je crven dok poruku nije proslijedio nijedan repetitor, a zelen od jednog naviše.

## 1.1.1
- **Redoslijed kanala**: drži kanal u kartici Kanali i povuci ga gore ili dolje da promijeniš redoslijed. Držanje bez pomicanja i dalje otvara izbornik kanala, u kojem je sada i **Vrati izvorni redoslijed**.
- Redoslijed se mijenja i sprema **samo u aplikaciji**, posebno za svaki node, i ostaje nakon ponovnog spajanja i ponovnog pokretanja aplikacije. Na node se ništa ne zapisuje: kanali na nodeu ostaju na svojim mjestima, a druge aplikacije spojene na isti node zadržavaju svoj redoslijed.
- **Bluetooth pretraga** prikazuje dva popisa: **U dometu** (nodeovi koje je pretraga pronašla, od najjačeg signala, s crticama signala i dBm, označeni kao *spremljen* ili *novi*) i **Spremljeni – nisu u dometu** (upareni ili spremljeni nodeovi koje pretraga nije pronašla, sivi, ali se i dalje mogu odabrati). Pretraga se pokreće sama kad otvoriš karticu Bluetooth, a spremljeni Bluetooth nodeovi više se ne prikazuju dvaput. Prikazani signal je izglađen (medijan zadnjih očitanja), pa crtice više ne titraju, a i Bluetooth nodeovi upareni samo u Androidu mogu se ukloniti s popisa (uz prečac do postavki Bluetootha za raskidanje uparivanja).
- Spremljeni nodeovi (WiFi, Tailscale, USB i Bluetooth) više nemaju ikonu za brisanje: drži node da ga ukloniš, a aplikacija prije toga traži potvrdu.
- Ispravljeno: brisanje nodea na koji se aplikacija još spajala nije zaustavljalo pokušaje, a „Odustani” odmah nakon pokretanja mogla je poništiti pozadinska usluga ponovnim spajanjem.
- Ispravljeno: „Proslijedilo repetitora” ostajao je na 0 na kanalu koji postoji u više mjesta s istim ključem, npr. drugi „Public” koji se koristi sa scopeom.
- Izraz „čuti” zamijenjen je u cijeloj aplikaciji, npr. „Zadnje detektirani”, „Detektirani kanali koje nemaš”, „Detektiran je kanal …”, „Proslijedilo repetitora: N” i „Tvoj signal kod repetitora” (i na srpskom).

## 1.1.0
- **Mađarski** jezik (Postavke → Izgled → Jezik → Magyar).
- **Čuti #kanali koje nemaš**: aplikacija prepoznaje promet na #kanalima koji nisu dodani (ugrađeni popis čestih kanala, gradova i regija, tvoja imena i kanali spomenuti u porukama) i javlja obavijest jednom po kanalu, s gumbima **Dodaj** i **Ne obavještavaj više**. Isti kanali prikazani su na vrhu kartice Kanali, pa dodaješ samo one koje želiš.
- Postavke → Obavijesti: uključivanje i isključivanje tih obavijesti, vlastita imena kanala za praćenje i reset utišanih kanala.
- Postavke → O aplikaciji: link **Popis promjena** ispod verzije aplikacije otvara promjene te verzije.
- Dodavanje i brisanje kanala sada je trenutno (aplikacija više ne čita ponovno sva mjesta za kanale s nodea).
- Opisi ikona koje čita čitač ekrana sada su na odabranom jeziku.
- Ispravljeno: tip kontakta senzor prikazivao se kao „Sensor” na hrvatskom i srpskom.

## 1.0.9
- Susjedni repetitori: status signala za svaki repetitor – ocjena (odličan / dobar / slab / vrlo slab) uz SNR i RSSI, koliko dobro repetitor čuje tebe, udaljenost te prosječni, najniži i najviši SNR.
- Susjedni repetitori: razvrstavanje po zadnjem čutom, najjačem signalu ili najbližem.
- Susjedni repetitori koji još nisu u kontaktima mogu se dodati jednim dodirom (ili svi odjednom); aplikacija prvo od repetitora dohvati njegov puni naziv.
- Kratki kod (1 bajt) spaja se s repetitorom koji je već prepoznat po duljem kodu; ako i dalje odgovara više repetitora, dodir na upitnik objasni o kojima se radi, najbliži prvi.

## 1.0.8
- Novi ekran **Susjedni repetitori** u izborniku ⋮ (ispod Primljeni adverti): repetitori koje tvoj node čuje izravno, s punim imenima kad su poznata, SNR-om, RSSI-jem, vremenom kad su zadnji put čuti i brojem paketa koji su stigli preko njih. Gumb za osvježavanje pita repetitore u dometu da se jave.

## 1.0.7
- Tipka za slanje adverta: kratki pritisak šalje zero-hop advert, a dugi pritisak flood advert.
- Tailscale → Uređaji u tailnetu: dodirom na uređaj spajaš se na MeshCore node na njemu (prvo traži potvrdu; TCP port se može promijeniti, zadano 5000).

## 1.0.6
- Broj novih primljenih adverta prikazuje se samo uz "Primljeni adverti" u izborniku ⋮, a ne više na ikoni izbornika.

## 1.0.5
- Ispravljene obavijesti: servis za vezu u pozadini sad se uvijek pokreće, pa poruke i obavijesti stižu i nakon izlaska iz aplikacije.
- Razgovor ostavljen otvoren u pozadini sad javlja nove poruke i ostavlja ih nepročitanima dok se ne vratiš.
- Postavke → Obavijesti upozoravaju kad su obavijesti za aplikaciju isključene u Androidu, s prečacem za uključivanje.

## 1.0.4
- Gumb za slanje adverta koristi simbol ((•)), kao u originalnoj aplikaciji.
- Pretraga kontakata otvara se iz gornje trake (ikona povećala) umjesto stalnog polja za pretragu.
- Primljeni adverti premješteni su u izbornik ⋮, s brojačem novih nodeova.

## 1.0.3
- Obavijest o vezi umjesto Bluetooth adrese prikazuje bateriju nodea i, preko Bluetootha, jačinu signala (preko WiFi-ja: LAN ili Tailscale).
- Obavijest o vezi više ne dodaje brojač nepročitanih na ikonu aplikacije.

## 1.0.2
- Polje za pretragu izgleda kao gumbovi kategorija ispod njega (isti rub i zaobljenost, manja visina) i ima gumb za brisanje.

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
- Gumb **Nepročitano**: pokazuje koliko razgovora ima nepročitane poruke i vodi ravno u najnoviji.
- Putanja poruke na karti crta se crvenom isprekidanom crtom sa strelicama smjera.
- Ispravke izgleda za Android 15 (nema praznog prostora iznad popisa).

## 0.7.0
- Broj repetitora koji su čuli tvoju poruku u kanalu, s popisom repetitora i njihovim SNR-om.
- Dugi pritisak na poruku: odgovori (@spominjanje), kopiraj, putanja na karti, pošalji ponovno, obriši.
- **Putanja poruke na karti**: repetitori kroz koje je poruka prošla.
- **Kontrola rute za DM**: automatski, uvijek flood ili ručna putanja preko odabranih repetitora.

## 0.6.0
- Opcija **Zapamti lozinku** za prijavu na repetitor i chat sobu (sprema se samo na telefonu).
- Obavijesti koriste ikonu aplikacije.

## 0.5.0
- Službeni simboli MeshCore nodeova na karti, obojeni prema tome koliko je davno node zadnji put čut.

## 0.4.0
- Nova ikona aplikacije.
- **Engleski** jezik (prebacivanje u Postavkama, uz hrvatski).
- Podaci o autoru u Postavke → O aplikaciji.

## 0.3.0
- **Automatski odabir veze**: kod kuće se aplikacija spaja izravno preko WiFi-ja, izvan kuće preko Tailscalea – ništa ne treba ručno prebacivati.
- Jednostavni, okrugli simboli nodeova na karti.

## 0.2.0
- Aplikacija se sad zove **MeshCore Go**.
- Spajanje na nodeove **preko lokalne mreže bez Tailscalea, preko Bluetootha LE i preko USB-a**.
- Zasebni simboli na karti za companion nodeove, repetitore, chat sobe i senzore.
- Podesiva **veličina fonta** i izbor fonta.
- **Stalni rad u pozadini**: zanemaruje štednju baterije, drži vezu s nodeom i **automatski se ponovno spaja** (svaka opcija se može uključiti ili isključiti).

## 0.1.0 – prva verzija
- Android MeshCore klijent s **ugrađenim Tailscaleom**: ne treba zasebna Tailscale aplikacija ni sistemski VPN. Prijava Tailscale auth ključem ili preko preglednika.
- Spajanje na WiFi companion node preko TCP-a, kroz tvoj tailnet.
- Kontakti, kanali i privatne poruke s potvrdom isporuke; chat sobe.
- Administracija repetitora: prijava, status, trace i CLI konzola.
- Karta nodeova.
- Raspored i tijek rada kao u originalnoj MeshCore aplikaciji (Kontakti, Kanali, Karta, Postavke), u vlastitom dizajnu.
