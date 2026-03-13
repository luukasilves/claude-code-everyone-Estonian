# Tund 1.4: Käsud ja navigeerimine

Enne kui teeme raske analüüsi, õpime kiiresti liikuma.

See tund käsitleb käske, kiirklahve ja mõningaid võimskasutaja funktsioone.

STOP: Valmis saama võimskasutajaks?

USER: Jah

---

## Olulised kaldkriipsu-käsud

Näitan sulle olulisi kaldkriipsu-käske.

Kirjuta lihtsalt `/`, et neid kõiki näha. Siin on peamised:

- **/model** - vaheta Claude'i mudelite vahel (Sonnet on kiire, Opus on tark)
- **/context** - vaata, millistest failidest Claude teadlik on
- **/clear** - alusta vestlust puhtalt lehelt
- **/compact** - tihenda vestlus konteksti säästmiseks
- **/usage** - vaata, kui palju oled kasutanud
- **/resume** - jätka sealt, kus eelmises sessioonis pooleli jäid

Täielik nimekiri on viitematerjalides.

STOP: Kirjuta `/`, et näha käskude menüüd. Näed neid?

USER: Jah

---

## Kohandatud käsud

Need olid sisseehitatud käsud. Aga siin on saladus: sa oled KOHANDATUD käske kasutanud kogu selle aja.

Iga kord, kui sa kirjutasid /start-1-1 või /start-1-2, oli see kohandatud käsk, mille ma selle kursuse jaoks lõin!

Kohandatud käsud elavad kaustas `.claude/commands/` - vaata seda kausta, kui oled uudishimulik.

See on põhimõtteliselt sama kontseptsioon nagu mallid, mida me varem kasutasime - fail juhistega, mis laetakse, kui sa selle välja kutsud. Otsetee asjadele, mida sa korduvalt teed.

Me ei süvene selles moodulis oma käskude loomisse, aga sa saad alati paluda mul käsu teha.

Üks oluline asi: kui sa lisad uusi käske, pead Claude Code'ist väljuma ja selle uuesti käivitama, et need ilmuksid.

STOP: Nipp: pärast taaskäivitust kasuta /resume, et jätkata täpselt sealt, kus pooleli jäid. Nii ei kaota sa oma vestlust. Selge?

USER: Jah

---

## Escape katkestamiseks

Siin on veel üks - Escape katkestamiseks.

Väga kasulik, kui muudad meelt või näed, et ma teen midagi valesti.

Proovime järele. Ma alustan pikka ülesannet ja sa saad mind igal hetkel peatada, vajutades Escape.

Sa pead mulle ütlema, et tegid seda, kuna see peatab mu.

ACTION: Start listing files recursively or doing something that takes a while and can be interrupted.

STOP: Vajuta Escape, et mind katkestada, ja ütle mulle, et tegid seda.

USER: Katkestasin su

Suurepärane! Sina oled kontrolli all. See on oluline - sa saad lasta mul töötada, jälgida, mida ma teen, ja peatada mind hetkel, kui midagi tundub vale. Palju parem kui oodata, kuni ma lõpetan vastuse, mida sa ei tahtnudki.

STOP: See säästab sul nii palju aega, kui sellega harjud. Valmis järgmiseks trikiks?

USER: Jah

---

## Tagasikerimise funktsioon

Tagasikerimise funktsioon: Esc×2 viimaste toimingute tagasivõtmiseks.

Sa saad kas AINULT vestluse lähtestada, aga säilitada kogu mu tehtud töö, või lähtestada nii koodi KUI KA vestluse.

See on nagu ajareisimine! Kasulik, kui tahad mingit rada uurida ja omada võimalust tagasi minna.

STOP: Proovi kohe - vajuta kaks korda Escape. Mida sa näed?

USER: Kirjeldab tagasikerimise valikuid

Täpselt! Järgmine kord, kui siia jõuad, ütle mulle, et oled seda juba teinud.

STOP: Tagasikerimine on su turvavõrk. Tahad midagi riskantset proovida? Anna minna - sa saad alati tagasi kerida. See on nagu piiramatult tagasivõtmine AI-tööle. Saad aru?

USER: Jah

---

## Mõtlemise märksõnad

Sa saad aidata mul teada, kui intensiivselt ma peaksin mõtlema, kasutades "think" märksõnu.

- "think about X" - tavaline mõtlemine
- "think harder" - sügavam analüüs
- "ultrathink" - maksimaalne mõtlemisvõimsus (näed vikerkaart!)

Kasuta neid, kui vajad, et ma päriselt mõne keerulise asja läbi töötaksin, aga ole ettevaatlik - tugev mõtlemine kulutab kasutuslimiite kiiremini.

STOP: Nipp: "ultrathink" on suurepärane strateegiliste otsuste, keerulise analüüsi jaoks või siis, kui mu esimene vastus tundub liiga pealiskaudne. See on nagu paluda kellelgi päriselt ühe probleemiga istuda, selle asemel et kiire vastus anda. Kirjuta see, et näha vikerkaart!! Siis anna mulle teada, kui oled valmis jätkama.

USER: Jah

---

## Kolm sisestusrežiimi

Kiire märkus sisestusrežiimide kohta. Claude Code'il on kolm:

- **Edit režiim** on vaikimisi. Ma küsin luba enne muudatuste tegemist. Turvaline, aga aeglasem.
- **Auto-accept režiim** tähendab, et ma lihtsalt teen. Kiirem, aga sa usaldad mind rohkem.
- **Plan režiim** tähendab, et ma loon esmalt plaani, sa vaatad selle üle, siis ma teostan.

Sa vahetad nende vahel Shift+Tab'iga.

Meie tegevuste jaoks on Edit või Auto režiim sobiv. Plan režiim on kasulik väga keeruliste mitmeetapiliste ülesannete jaoks, aga ausalt öeldes saad tavaliselt plaani minuga lihtsalt vestluses läbi arutada. Tulevikus vaatame üle ka AskUserQuestions tööriista, mis on prototüüpimise jaoks väga abiks, sest ma saan aidata sul KÕIK läbi mõelda. Aga selle taseme töö jaoks pole seda vaja.

STOP: Enamik inimesi alustab Edit režiimis turvalisuse pärast, siis läheb üle Auto režiimile, kui usaldavad töövoogu. Sa leiad oma mugavustaseme. Valmis salajaseks võimurežiimiks?

USER: Jah

---

## Suur finaal: Lubade ohtlik vahelejätmine

Olgu, nüüd suur finaal. Salajane võimurežiim.

Selle asemel, et käivitada Claude Code lihtsalt käsuga `claude`, saad käivitada: `claude --dangerously-skip-permissions`

See käivitab Claude Code'i ILMA ühegi loanõudeta. Ma lihtsalt teen kõike. Kinnitusdialooge pole, heakskiidu küsimist pole.

Seda kutsutakse "ohtlikuks" põhjusega - sa annad mulle täieliku kontrolli. Aga kui sa usaldad, mis toimub, on see NII palju kiirem.

Carl (kursuse looja) kasutab seda režiimi peaaegu eranditult, kaasa arvatud selle kursuse ehitamiseks! Kui sa oled Claude Code'iga mugavaks saanud, kasutad tõenäoliselt sinagi. Vaata viitejuhendist nippe, kuidas seda turvalisena hoida.

STOP: Tunned end võimsana?

USER: Jah

---

## Kokkuvõte

**Põhioskused, mida just õppisid:**

1. **Kaldkriipsu-käsud:** Kiired juhtelemendid mudelite, konteksti, tühjendamise, jätkamise jaoks
2. **Kohandatud käsud:** Loo oma otseteed korduvate töövoogude jaoks (nagu /start käsud selles kursuses)
3. **Katkestamine ja tagasikerimine:** Kontrolli säilitamine, uurimine ilma siduvuseta
4. **Mõtlemise märksõnad:** Sügavam analüüs, kui seda vajad
5. **Lubade ohtlik vahelejätmine:** Täiskiiruse režiim, kui usaldad protsessi

**Kus seda veel rakendada:**
- Iga kord, kui töötad kiiresti ja usaldad Claude'i - jäta loanõuded vahele
- Kui vajad sügavamat mõtlemist keerulise probleemi üle - kasuta mõtlemise märksõnu
- Kui midagi läheb valesti - keri tagasi ja proovi teist lähenemist
- Kui tahad puhtalt alustada - /clear ja alusta uuesti

**Järgmisena:** Tunnis 1.5 läheb asi põnevaks. Sa õpid agentide kohta - võime käivitada mitu Claude'i instantsi, mis töötavad paralleelselt. Me töötleme kõik need konkurentide failid ja vanad kampaaniad korraga läbi. Siit hakkab Claude Code tunduma nagu supervõime.

STOP: Valmis tunniks 1.5?

USER: Jah / /start-1-5

---

## Olulised märkmed Claude'ile

- **Escape demo**: Alusta midagi katkestatavat, et õpilane saaks päriselt harjutada Escape vajutamist
- **Tagasikerimise demo**: Lase neil proovida Esc×2 ja näha valikuid
- **Ära müü Plan režiimi üle**: Me oleme seda tahtlikult tagaplaanile jätnud - see on kasulik, aga mitte kriitilise tähtsusega selle taseme töö jaoks
- **Lubade ohtlik vahelejätmine**: Rõhuta, et see on usaldusväärsete töövoogude jaoks, mitte kõige jaoks

## Edukuse kriteeriumid

- [ ] Õpilane teab peamisi kaldkriipsu-käske (/model, /clear, /compact, /resume)
- [ ] Õpilane mõistab, et kohandatud käsud elavad kaustas .claude/commands/
- [ ] Õpilane on harjutanud katkestamist Escape'iga
- [ ] Õpilane on näinud tagasikerimise valikuid
- [ ] Õpilane teab mõtlemise märksõnadest
- [ ] Õpilane mõistab kolme režiimi (Edit, Auto, Plan)
- [ ] Õpilane on kuulnud --dangerously-skip-permissions kohta
- [ ] Õpilane on valmis tunniks 1.5
