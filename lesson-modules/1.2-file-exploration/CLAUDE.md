# Tund 1.2: Failide uurimine ja visualiseerimine

Olgu, NÜÜd astume stsenaariumisse.

Sa armastad kohvi. Nagu, päriselt armastad. Nii et kui sa nägid Basecamp Coffee juhi kohta kuulutust, haarasid sellest kohe kinni.

Basecamp Coffee on piirkondlik kett - umbes 45 asukohta üle Pacific Northwest'i. Head oad, hubane atmosfäär, lojaalsed püsikliendid.

Aga hoiatus: eelmine juht oli... noh, mitte just parim. Asjad on üsna sassis. Märkmed igal pool. Pooleli jäänud projektid. Lojaalsusprogramm, mis ilmselt põletab raha.

Aga hei - just seepärast nad su palkasidki. Aeg välja selgitada, mis toimub.

STOP: Valmis nägema, mida sa pärisid?

USER: Jah

---

## Uuri failistruktuuri

Vaatame, millega sa tööle hakkad. Palu mul näidata sulle failistruktuuri.

STOP: Ütle "Näita mulle failistruktuuri"

USER: Näita mulle failistruktuuri

ACTION: Run `ls -la` and show the main folders. Explain: "Sul on olemas company-context (taustainfo), inherited-chaos (pärandatud segadus), templates ja attachments."

[Show the file tree in ASCII]

STOP: Näed, kuidas on kaks peamist kausta? `company-context` ja `inherited-chaos`? Palu mul ettevõtte kontekst kokku võtta.

USER: Võta ettevõtte kontekst kokku

---

## Loe kontekstifaile

ACTION: Read the three files in company-context/ and give a conversational summary:
- SCENARIO.md: Su olukord - 3 kuud, et pöörata ümber läbikukkuv lojaalsusprogramm
- LOYALTY-PROGRAM.md: Praegune programmi struktuur ja (halvad) mõõdikud
- BRAND-VOICE.md: Kuidas Basecamp suhtleb

Pane tähele, kuidas ma just lugesin mitu faili ja andsin sulle kokkuvõtte? Sa saaksid sama asja teha ükskõik millise dokumendikaustaga - lepingud, uurimistööd, koosolekute märkmed. Lihtsalt suuna mind nende poole ja palu kokkuvõtet.

STOP: Kas sul on küsimusi ettevõtte konteksti kohta enne, kui piilume kaosesse?

USER: Vastab

---

## Piilu kaosesse

Nüüd piilume pärandatud kaosesse. Mis siin sees on?

ACTION: Run `ls inherited-chaos/` and describe what you see - segased märkmed, klientide tagasiside, konkurentide uuringud, vanad kampaaniad ja CSV andmetega.

Näed, mis segaduse sa pärisid? Kaevume sellesse hiljem sügavamale.

Sa võid olla natuke segaduses - ma loen neid faile ja räägin sulle, mis neis on, aga kuidas sa ise neid näed ja nendega töötad?

Seadistame su tööruumi.

STOP: Valmis seadistama tööruumi, kus sa päriselt kõike seda näed?

USER: Jah

---

## Sein

Nii, ilmselgelt on see terminal. Sa saad minuga siin töötada, aga faile visuaalselt sirvida ei saa.

Failide vaatamiseks läheb sul vaja redaktorit. Mul on kaks soovitust:

**Valik 1: Nimbalyst (Soovitatud)**
- Spetsiaalselt loodud mittetehnilistele Claude Code'i kasutajatele
- Ilus redaktor failide vaatamiseks ja muutmiseks
- Claude Code on sisse ehitatud
- Tasuta allalaaditav
- See on Carl'i soovitus

**Valik 2: Cursor**
- Koodiredaktor (aga töötab suurepäraselt kõigi failidega)
- Omab enda AI-funktsioone, mida saad Claude Code'i kõrval kasutada
- Tasuta allalaaditav

STOP: Kumba soovid kasutada? Ütle **'Nimbalyst'** või **'Cursor'**

USER: Nimbalyst / Cursor

---

## Nimbalyst'i seadistamine

[Kui kasutaja valis Nimbalyst'i:]

Suurepärane valik! Seadistame Nimbalyst'i.

**Samm 1: Laadi Nimbalyst alla**

Mine aadressile: **https://nimbalyst.com/**

Klõpsa allalaadimise nuppu oma operatsioonisüsteemi jaoks (Mac, Windows või Linux).

**Samm 2: Paigalda**

- **Mac:** Ava .dmg fail ja lohista Nimbalyst Applications kausta
- **Windows:** Käivita paigaldaja ja järgi juhiseid
- **Linux:** Järgi allalaadimislehel olevaid paigaldusjuhiseid

**Samm 3: Ava Nimbalyst**

Käivita Nimbalyst. Näed peamist liidest.

STOP: Anna mulle teada, kui Nimbalyst on avatud. Ütle **'Nimbalyst on avatud'**

USER: Nimbalyst on avatud

---

## Ava kursuse kaust Nimbalyst'is

Nüüd peame avama su kursuse kausta.

ACTION: Run `pwd` to get the current directory path

Su kursuse kaust asub:
**[näita täielik tee]**

Nimbalyst'is:
1. Otsi valikut kausta või projekti avamiseks
2. Navigeeri ülal näidatud teele
3. Vali see ja ava

Sa peaksid nägema oma faile külgribal - kaustad nagu `company-context/`, `inherited-chaos/` jne.

STOP: Kas sa näed kursuse faile? Ütle **'Ma näen faile'**

USER: Ma näen faile

---

## Jätka tundi Nimbalyst'is

Suurepärane! Nüüd tuleb oluline osa.

Nimbalyst'il on Claude Code sisse ehitatud. Sa peaksid nägema terminali või vestlusliidest, kus saad Claude'iga rääkida.

Leia see liides ja kirjuta:
```
/start-1-2
```

See jätkab tundi täpselt sealt, kus pooleli jäime, aga nüüd Nimbalyst'i sees, kus sa näed oma faile!

STOP: Kirjuta `/start-1-2` Nimbalyst'is ja ütle siis **'Ma olen Nimbalyst'is!'**

USER: Ma olen Nimbalyst'is!

---

## Cursor'i seadistamine

[Kui kasutaja valis Cursor'i:]

Lubage tutvustada sulle Cursor'it. See on koodiredaktor, mis näitab su faile töö ajal. Muidugi, nagu Claude Code, saab seda kasutada palju enamaks kui kood. See on lihtsalt viis igasuguste failide vaatamiseks ja nendega töötamiseks.

See on tasuta ja populaarne ning omab enda AI-funktsioone, mida saad minu kõrval kasutada.

Cursor'il on oma AI-funktsioonid, aga need on täiesti eraldi terminalist, kus Claude Code elab. Sul ei ole vaja Cursor'i tellimust.

Need järgmised sammud on kõige hirmutavamad kogu sellest kogemusest, aga sa suudad palju raskemaid asju kui see.

STOP: Mine laadi Cursor alla aadressilt cursor.com ja paigalda see. Vaata viitedokumenti üksikasjalike juhiste jaoks. Anna mulle teada, kui soovid, et avaksin allalaadimislehe. Ütle, kui Cursor on paigaldatud.

USER: Tehtud

---

## Ava kursuse kaust Cursor'is

[Kui kasutaja on macOS-il (platform = darwin):]

ACTION: Run `open -a "Cursor" "[current working directory]"` to open the folder directly in Cursor.

Avasin just kursuse kausta Cursor'is sinu eest.

**Oluline:** Cursor võib vaikimisi avada "Agents" vaates - näed vestlusliidest failide asemel. Vaata päris ülemisse vasakusse nurka ja klõpsa **"Editor"**, et lülituda failide vaatesse. Seejärel peaksid nägema kursuse faile külgribal.

[Kui kasutaja on Windows'il (platform = win32):]

Nüüd ava Cursor ja klõpsa "Open project", et avada kursuse kaust.

Su kausta tee on: [current working directory]

**Oluline:** Cursor võib vaikimisi avada "Agents" vaates - näed vestlusliidest failide asemel. Vaata päris ülemisse vasakusse nurka ja klõpsa **"Editor"**, et lülituda failide vaatesse.

[Kui kasutaja on Linux'il (platform = linux):]

Nüüd ava Cursor ja klõpsa "Open project", et avada kursuse kaust.

Su kausta tee on: [current working directory]

**Oluline:** Cursor võib vaikimisi avada "Agents" vaates - näed vestlusliidest failide asemel. Vaata päris ülemisse vasakusse nurka ja klõpsa **"Editor"**, et lülituda failide vaatesse.

STOP: Kas sa näed Cursor'it avatuna kursuse failidega külgribal?

USER: Jah

---

## Käivita Claude Code Cursor'i sees

Nüüd käivitame Claude Code'i Cursor'i sees.

Veendu, et oled "Editor" vaates, MITTE "Agents" - näed neid valikuid päris ülemises vasakus nurgas.

Seejärel pead avama terminali Cursor'i sees.

Vajuta `Ctrl+`` (see on backtick-klahv, tavaliselt Tab-klahvi kohal, kus on ka laineline ~). Või mine menüüs View → Terminal.

Sa peaksid nägema paneeli, mis ilmub Cursor'i alaossa. See on su terminal.

Kui see on avatud, kirjuta `claude` ja vajuta Enter. See käivitab minu uue instantsi seal.

Kui näed Claude Code'i käivitumist, kirjuta `/start-1-2`, et jätkata seda tundi.

STOP: Cursor'is kirjuta /start-1-2 ja ütle, et oled Cursor'is!

USER: Ma olen Cursor'is!

---

## Kontrolli failide nähtavust

Võimas töö! See oli kogu selle kogemuse kõige konarlikum osa. Siit edasi on kõik sujuv sõit.

Näitan sulle ringi.

Vasakul paneelil peaksid nägema neid kursuse faile. Kui sa neid ei näe, oled võib-olla "Agents" vaates ülemises vasakus nurgas. Sa pead olema "Editor" vaates.

STOP: Kas sa näed seal faile?

USER: Kinnitab

---

## Räägime failidest

Leia kaust 'company-context' - kas sa näed kolme faili sees?

Failis BRAND-VOICE.md on päris alguses salasõna. Vaata, kas leiad selle üles.

STOP: Mis on salasõna?

USER: COFFEE

---

## Selgitame Markdown-faile

Tubli! See, mida sa näed, on markdown ehk .md fail, mis on lihtsalt väga levinud dokumentide standard. LLM-id armastavad markdown-faile.

Sa saad seda ilusamalt vaadata, avades selle Cursor'is Preview režiimis. Tee failile faililoendis paremklõps ja klõpsa Preview.

STOP: Kas see töötas sul?

USER: Jah

---

## Demonstreerime faili loomist

Tore! Sa saad kasutada ka Cmd/Ctrl+Shift+V, et avada Preview.

Olgu, see oli failide vaatamine. Muidugi, ma saan faile ka luua.

STOP: Palu mul luua testfail, mis mõnitab ChatGPT-d.

USER: Loo testfail, mis mõnitab ChatGPT-d

ACTION: Create a file called `test-file.md` with fun content roasting ChatGPT, and put the secret word "ESPRESSO" at the very top.

Olgu, panin jälle salasõna algusesse. Kas leiad selle?

STOP: Mis on salasõna?

USER: ESPRESSO

---

## Kehtestame töövoo

See olen mina, espesso! Sa hakkad pihta saama.

See ongi töövoog: sul on alati oma failid, oma tööruum ja mina terminalis, töötame koos.

Nüüd sa NÄED töö ajal.

STOP: Tunned end mugavalt selle seadistusega?

USER: Jah

---

## Kokkuvõte

**Põhioskus:** Võõraste failistruktuuride uurimine ja tööruumi seadistamine, kus sa näed, mis toimub.

**Kus seda veel rakendada:**
- Sa pärid projekti kolleegilt, kes lahkus - segased kaustad, dokumentatsioon puudub. Claude saab selle kaardistada ja selgitada, mis kõik on.
- Klient saadab sulle zip-faili oma "brändimaterjalidega" - 17 kausta, ebajärjekindel nimetamine. Saa minutitega selgust, mitte tundidega.
- Su enda Downloads kaust on muutunud kalmistuks. Suuna Claude sinna: "Mis siin on? Mida saan kustutada?" (Suurepärane viis kettaruumi vabastamiseks.)
- Alustad uut tööd ja pead mõistma, kuidas tiim oma jagatud ketast korraldab.
- Laadisid alla kursuse või ressursipaki ja tahad aru saada, mis seal tegelikult sees on, enne kui sisse sukeldud.

**Järgmisena:** Tunnis 1.3 kaevume päriselt pärandatud kaosesse. Sa õpid, kuidas segastest dokumentidest teadmisi ammutada, mustreid kaustade üleselt sünteesida, pilte analüüsida ja veebiuuringuid teha - kõik lihtsate @ mainingutega. Hakkame avastama, mis selle lojaalsusprogrammiga tegelikult valesti on.

STOP: Valmis tunniks 1.3?

USER: Jah / /start-1-3

---

## Olulised märkmed Claude'ile

- **Tee tuvastamine**: Kui ütled kasutajale kausta teed, tuvasta nende tegelik töökataloog
- **Platvormi tuvastamine**: Kontrolli `Platform:` välja keskkonna infos. Kasuta macOS-il (darwin) `open -a "Cursor" "/path/to/folder"`, et avada Cursor otse. Windows'i (win32) ja Linux'i kasutajad peavad kasutama käsitsi File → Open Folder.
- **Cursor'i juhendamine**: Kui kasutaja on juba Cursor'is/VS Code'is, jäta allalaadimise osa vahele
- **Agents vaate segadus**: Cursor avab vaikimisi "Agents" vaate, mis näitab vestlusliidest, mitte faile. Kui kasutaja on segaduses, kus failid on, või ei näe külgriba, on ta tõenäoliselt Agents vaates. Juhi ta klõpsama "Editor" päris ülemises vasakus nurgas. Cursor reklaamib Agents vaadet, aga see ei tööta selle kursuse jaoks - meil on vaja failiuurijat.
- **Salasõnad**: BRAND-VOICE.md-s peab olema ülaosas "COFFEE"; test-file.md saab "ESPRESSO"
- **Kannatlikkus**: Cursor'i seadistamine võib mittetehnilistele kasutajatele segane olla. Mine aeglaselt, paku abi veaotsingul
- **Faili loomine**: Loo päriselt test-file.md - ära ainult kirjelda seda

## Edukuse kriteeriumid

- [ ] Õpilane mõistab Basecamp Coffee stsenaariumit ja oma rolli
- [ ] Õpilasel on Cursor (või VS Code) avatud kursuse kaustaga
- [ ] Õpilane näeb faile külgribal
- [ ] Õpilane leidis mõlemad salasõnad (COFFEE, ESPRESSO)
- [ ] Õpilane mõistab töövoogu: failid + redaktor + Claude terminalis
- [ ] Õpilane on valmis liikuma tunni 1.3 juurde
