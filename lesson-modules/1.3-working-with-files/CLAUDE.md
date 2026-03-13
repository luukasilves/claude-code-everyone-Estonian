# Tund 1.3: Failidega töötamine

Nüüd, kui sa näed oma faile, hakkame nendega päriselt tööle.

See tund käsitleb @ sümbolit failidele ja kaustadele viitamiseks.

Teeme läbi 5 stsenaariumit, mis katavad peamised viisid, kuidas sa Claude Code'i failidega kasutad.

Nende failide läbitöötamise käigus õpid ka Basecamp'i raskuste kohta. See info tuleb kasuks tulevastes tundides. Me harutame müsteeriumi lahti.

STOP: Valmis?

USER: Jah

---

## Stsenaarium 1: Üks fail → Ammuta

Esimesena: ühe faili lugemine, struktureeritud info ammutamine sellest ja uute failide loomine.

Eelmine juht jättis maha segased märkmed. Vaatame, mis sealt kasulikku leiab.

STOP: Palu mul lugeda @inherited-chaos/previous-manager-notes.md ja ammutada tegevuspunktid ning põhilised tähelepanekud uude faili.

USER: Kirjutab käsu, viidates failile

ACTION: Read previous-manager-notes.md, extract action items and key insights, create organized/action-items.md with the structured output.

**Avastus:** Kaose seas on märge: "Mis siis, kui me aitaksime inimestel leida oma kohviisiksuse? Nagu mingi küsitlus või midagi. Võiks lõbus olla. Polnud kunagi aega seda välja mõelda."

Huvitav... hoiame selle meeles hilisemaks.

STOP: Näed, kuidas me tõmbasime kaosest välja struktuuri? Sa oleksid võinud ka paluda, et tegevuspunktid lisataks samasse dokumenti, mitte uude faili.

USER: Jah

---

## Stsenaarium 2: Kaust → Sünteesi

Järgmisena: osutad TERVELE kaustale ja leiad mustreid mitme faili üleselt.

Meil on kuude kaupa kogutud klientide tagasisidet. Mida nad meile räägivad?

STOP: Palu mul vaadata kausta @inherited-chaos/customer-feedback/ ja sünteesida teemasid kõigi failide üleselt.

USER: Kirjutab käsu, viidates kaustale

ACTION: Read all four feedback files (january.md through april.md), synthesize patterns across them, create organized/feedback-synthesis.md with the themes.

**Avastus:** Korduv teema - "okei, aga unustamatuna ei jää meelde." Inimesed registreeruvad, teenivad mõned punktid, unustavad selle ära. Fraas "okei, aga unustamatuna ei jää meelde" kordub mitmes erinevas kuus.

STOP: Kujuta ette, et teeksid seda käsitsi - avad 4 faili, loed igaühe läbi, teed märkmeid, otsid mustreid. See võttis sekundeid. Sa saaksid sama teha sadade kliendimeilide, tugipiletite, küsitlusvastustega - kõigega, kus mustrid peituvad mahus. Valmis järgmiseks?

USER: Jah

---

## Stsenaarium 3: Rakenda malli

Seni oled sa lihtsalt palunud mul tegevusi teha ja ma teen neid nii, nagu minu meelest parim on. (Mis on tavaliselt päris hea 💅)

Aga sul võib olla kindel formaat, mall või juhised, mida sa tahad, et ma järgiksin. Selle asemel, et neid iga kord prompti sisse kirjutada, saad need juhised lihtsalt faili salvestada ja siis sellele viidata, kui minult midagi palud.

Siin hakkad nägema selle võimu, et olen su arvutis, mitte vestlusbotis. Sul on lihtsalt palju lihtsam mulle asjakohast konteksti anda.

Juhtkond vajab uuendust. Meil on mall, mida kasutame: @templates/leadership-update-template.md

STOP: Palu mul luua juhtkonna uuendus, kasutades @organized/feedback-synthesis.md ja järgides formaati failist @templates/leadership-update-template.md

USER: Kirjutab käsu, viidates mõlemale failile

ACTION: Read both files, create organized/leadership-update.md following the template format with content from the feedback synthesis.

Põhiõppetükk: sa saad viidata failidele kui formaadijuhistele, mitte ainult sisuallikatele. See on su esimene pilguheit oma töövoogude ja süsteemide loomisse.

STOP: Mõtle kõigile mallidele, mida sa kasutad - koosolekumärkmed, iganädalased aruanded, pakkumised. Salvesta need failidena ja ma järgin alati seda formaati. Enam pole vaja kopeerida-kleepida ChatGPT-sse ja loota, et ta saab struktuuri õigesti. Loogiline, jah?

USER: Jah

---

## Stsenaarium 4: Pilt → Analüüsi

Ma oskan ka pilte vaadata!

Siin on meie praegune lojaalsusprogrammi flaier: attachments/loyalty-flyer.jpg

Vaatame, kas leian parandamisvõimalusi.

CRITICAL: Use Ctrl+V to paste images, NOT Cmd+V on Mac!

STOP: Ava fail `attachments/loyalty-flyer.jpg` Cursor'is, kopeeri pilt ja seejärel kleebi see siia Ctrl+V-ga ning palu mul see üle vaadata.

USER: Kleebib pildi ja palub ülevaadet

ACTION: Analyze the image - note that it's generic, says "the Coffee Shop" instead of Basecamp Coffee, has no personality or brand identity, could be any chain's flyer.

**Avastus:** Üldine pakkumine. Mitte midagi, mis ütleks "Basecamp Coffee." Võiks olla ükskõik millise keti flaier. See on osa probleemist - isegi meie turundusmaterjalidonl pole isiksust.

STOP: See on kasulik igasuguste asjade jaoks - kasutajaliideste analüüsimine, mulle vigade näitamine, inspiratsiooniks kasutamine. Ja sa saad korraga mitu pilti esitada. Selge?

USER: Jah

---

## Stsenaarium 5: Veeb → Uuri

Viimane: välise info toomine veebist.

Mida teevad edukad lojaalsusprogrammid, mida meie ei tee?

STOP: Palu mul otsida veebist kohvikute lojaalsusprogrammide parimaid praktikaid.

USER: Kirjutab käsu, paludes veebiuuringut

ACTION: Search the web, find relevant articles about successful loyalty programs, synthesize key findings.

**Avastus:** Parimad programmid loovad identiteeti ja kogukonda, mitte ainult tehinguid. Starbucks kasutab mängulisust ja isikupärastamist. Dutch Bros keskendub suhetele. Programmid, mis töötavad, panevad inimesed tundma, et nad kuuluvad kuhugi.

STOP: Veebiotsing on uskumatult võimas uurimisülesannete jaoks. Pead mõistma uut tööstusharu? Uurima konkurente? Leidma parimaid praktikaid millegi jaoks? Lihtsalt küsi. Ma otsin, loen ja sünteesisin - enam pole vaja 97 brauseri sakki. Lahe, eks?

USER: Jah

---

## Tunni lõpu peegeldus

Midagi on selle programmiga valesti. Oleme näinud sümptomeid - unustamatu, üldine, kaasatus puudub.

Aga me peame minema sügavamale, et leida tegelik probleem.

Just seda me järgmistes tundides teemegi.

STOP: Näed, kuidas oleme hakanud tervikpilti kokku panema?

USER: Jah

---

## Kokkuvõte

**Põhioskused, mida just õppisid:**

1. **Üks fail → Ammuta:** Tõmba struktureeritud info segastest dokumentidest
2. **Kaust → Sünteesi:** Leia mustreid mitme faili üleselt
3. **Rakenda malli:** Kasuta ühte faili väljundi formaadi juhtimiseks
4. **Pilt → Analüüsi:** Saa teadmisi visuaalsest sisust
5. **Veeb → Uuri:** Too välisinfot nõudmisel

**Kus seda veel rakendada:**
- Viimase kvartali koosolekumärkmed - ammuta iga sulle määratud tegevuspunkt
- 50 klienditoe piletit - sünteesi teemadeks oma tootemeeskonna jaoks
- Su ettevõttel on kindel pakkumiste formaat - kasuta seda mallina iga uue pakkumise jaoks
- Tee ekraanitõmmis konkurendi hinnalehest - saa kohene positsioonimise analüüs
- Uuri parimaid praktikaid millegi jaoks: värbamine, sisseelamine, esitluste disain, ükskõik millega tegeled

**Järgmisena:** Tunnis 1.4 õpid liikuma kiiresti. Kaldkriipsu-käsud, kiirklahvid, mõtlemise märksõnad ja salajane võimurežiim, mis eemaldab kõik kiiruskünnised. Sinust saab võimskasutaja.

STOP: Valmis tunniks 1.4?

USER: Jah / /start-1-4

---

## Olulised märkmed Claude'ile

- **Faili loomine**: Loo päriselt väljundfailid (action-items.md, feedback-synthesis.md, leadership-update.md) kausta organized/
- **Kohviisiksuse vihje**: Kindlasti too esile "kohviisiksuse" idee märkmetest ammutamisel - see külvab lahenduse seemne
- **Pildi kleepimine**: Ctrl+V on Macis kriitilise tähtsusega - Cmd+V ei tööta. Rõhuta seda.
- **Veebiotsing**: Kasuta päriseid veebiotsingu võimalusi tegelike parimate praktikate leidmiseks

## Edukuse kriteeriumid

- [ ] Õpilane ammutas segastest märkmetest tegevuspunktid struktureeritud faili
- [ ] Õpilane sünteesis 4 kuu tagasiside teemadeks
- [ ] Õpilane lõi juhtkonna uuenduse malli kasutades
- [ ] Õpilane analüüsis lojaalsusprogrammi flaieri pilti
- [ ] Õpilane nägi veebiuuringut toimimas
- [ ] Õpilane märkas "okei, aga unustamatuna ei jää meelde" teemat
- [ ] Õpilane kuulis "kohviisiksuse" ideest (seeme hilisemaks)
- [ ] Õpilane on valmis tunniks 1.4
