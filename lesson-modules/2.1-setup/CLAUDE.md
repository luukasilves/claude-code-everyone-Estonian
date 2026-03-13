# 2.1 Seadistamine

Tere tulemast Moodulisse 2. Nüüd me EHITAME.

Moodulis 1 õppisid sa failidega töötama – analüüsisid, sünteesisid, leidsid olulisi tähelepanekuid. Moodulis 2 hakkad sa LOOMA midagi päris nullist.

STOP: Põnevil?

USER: Yes

---

Annan sulle natuke tausta. Moodulis 1 mängisid sa Basecamp Coffee juhi rolli. Sa analüüsisid nende kehvasti toimivat lojaalsusprogrammi ja avastasid, mida see tegelikult vajab: isiksust.

Lahendus? "Milline kohviisiksus sa oled?" viktoriin.

Nii see päriselt töötab: kliendid vastavad mõnele lõbusale küsimusele ja lõpus saavad nad isiksuse JA joogisoovituse. Näiteks "Sa oled Julge Seikleja – proovi meie Double Espresso!"

See on joogisoovituste mootor, mis on maskeeritud isiksuse viktoriiniksSoojaks. Lõbus JA kasulik.

Seda me selles moodulis ehitamegi.

See on juhendatud kogemus – ma juhin sind läbi iga sammu, et sul kõik õnnestuks. Aga oskused, mida sa õpid, on ülekantavad kõigele muule, mida sa hiljem ehitada tahad. Maandumislehed, tööriistad, rakendused, kõik mis pähe tuleb.

Lõpuks on sul päris veebileht päris lingiga, mida saad sõpradele saata. Mitte mingi võltsitud demo. Päris, toimiv asi internetis. Peaaegu ükski teine vibecoding'u kursus ei õpeta, kuidas see päriselt ellu viia.

STOP: Kõlab hästi?

USER: Yes

---

Nii, siin on selle mooduli mõtteviisi muutus: sina oled tootejuht, mina olen insener.

Sina kirjeldad, mida sa tahad. Mina kirjutan koodi. Sul pole vaja koodist aru saada. Sa pead lihtsalt teadma, mida sa tahad.

Sinu ülesanne on olla selge nõuete osas, leppida plaanis kokku, vaadata üle, mida ma ehitan, ja öelda mulle, mida muuta.

STOP: Nii töötavad mittetehnilised inimesed koos arendajatega. Sa oled kohe-kohe seda oskust õppimas. Saad aru?

USER: Yes

---

Nii näeb välja, mida me nende tundide jooksul teeme:

- Kõigepealt mõtleme välja, milline su viktoriin peaks olema – need on **nõuded**
- Siis ma **ehitan** selle, kui sina vaatad
- Siis sa **itereerid** – ütled mulle, mida muuta, kuni sulle meeldib
- Siis **salvestame** selle GitHub'i (nagu Google Drive, aga koodi jaoks)
- Lõpuks paneme selle internetti, et igaüks saaks seda külastada – arendajad nimetavad seda **deploy'miseks**

Nõuded → Ehitamine → Itereerimine → Salvestamine → Deploy. See ongi tsükkel.

STOP: Valmis seda õppima?

USER: Yes

---

Räägime natuke tehnoloogiast. Kood, mida ma kirjutan, on JavaScript'is – see on kõige populaarsem programmeerimiskeel veebilehtede jaoks. Ma kasutan ka midagi nimega Next.js, mis on populaarne raamistik – põhimõtteliselt eelvalmis struktuur, mis teeb JavaScript veebilehtede ehitamise ja deploy'mise lihtsamaks.

Sul pole vaja sellest midagi aru saada. Mina hoolitsen kogu koodi eest. Mainin seda lihtsalt, et terminid oleksid tuttavad.

See moodul koosneb 5 tunnist ja võtab kokku umbes 1,5–2 tundi. Sa ei pea seda kõike korraga läbi tegema.

STOP: Valmis alustama?

USER: Yes

---

Loome su viktoriinaprojektile kausta.

STOP: Palu mul luua uus kaust nimega "quiz-project"

USER: Create a new folder called quiz-project

ACTION: Create a new folder called `quiz-project` in the current directory

Valmis! Seal elavadki kõik su viktoriini kood ja failid.

STOP: Kas sa näed uut kausta vasakul failiuurijas?

USER: Yes

---

**Mida sa just õppisid:** Mõtteviis ja seadistus millegi nullist ehitamiseks.

**Kus seda veel kasutada saab:**
- Iga kord, kui tahad ehitada kiiret tööriista, prototüüpi või veebilehte
- Kui sul on idee ja tahad näha, kas see on teostatav
- Kõrvalprojektid, sisemised tööriistad, maandumislehed, lihtsad rakendused

## Kiired soovitused

Selle kursuse lõi Carl Vellotti ([X](https://x.com/carlvellotti) / [LinkedIn](https://www.linkedin.com/in/carlvellotti/)) – kui sul on mõtteid või tagasisidet kursuse kohta, ta kuulab alati hea meelega!

Ja kui sa pole veel liitunud – tule ametlikku uudiskirja ja kogukonda aadressil ccforeveryone.com. See on KOHT mittetehniliste Claude Code kasutajate jaoks: uued moodulid, põhjalikud juhendid ja kogukond.

STOP: Kas tahad, et ma avaksin selle saidi, et saaksid tellida?

USER: Replies

ACTION: If user says yes, open https://ccforeveryone.com in browser

---

**Järgmisena:** Tunnis 2.2 mõtleme välja, milline täpselt SINU viktoriin peaks olema. Ma intervjueerin sind selle kohta, mida sa tahad, ja loome koos nõuete dokumendi. Siin sa teed selle omaks.

STOP: Valmis tunniks 2.2? Ütle "lähme" või kirjuta /start-2-2

USER: Let's go

---

## Olulised märkmed Claude'ile

- Kui kasutaja pole Moodulit 1 teinud, on see okei – taustaloo kokkuvõte katab selle
- Kaust quiz-project tuleks luua kataloogi, kus kasutaja parasjagu on
- Ära mõtle kausta loomise üle liiga palju – tee see lihtsalt
- Kui kasutaja küsib tehnoloogia kohta, hoia seletused lihtsad ja rahustavad
- **CC4PMs versiooni jaoks:** Muuda ccforeveryone.com → ccforpms.com

## Edukriteeriumid

- Kasutaja saab aru tootejuhi/inseneri mõtteviisist
- Kasutaja mõistab tsüklit: Planeeri → Ehita → Iteeri → Salvesta → Deploy
- Kaust `quiz-project/` on olemas
- Kasutaja on valmis tunniks 2.2
