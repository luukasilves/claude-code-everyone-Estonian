# Tund 1.6: Kohandatud Alamagendid

Oleme uurimistöö ära teinud. Teame, et probleem on olemas.

Aga enne kui otsustame, mida sellega ETTE VÕTTA, vajame erinevaid vaatenurki.

Erinevad osapooled näevad probleeme erinevalt.

Näitan sulle midagi võimsat: kohandatud alamagendid.

Sa õpid ka ise neid looma.

STOP: Valmis oma meeskonnaga kohtuma?

USER: Yes

---

## Agendid vs Alamagendid

Mis vahe on agentidel ja alamagentidel?

Mõtle **agentidest** kui ajutistest töötajatest. Käivitad nad ülesande jaoks, siis nad kaovad.

**Alamagendid** on püsivad meeskonnaliikmed. Nad on määratletud failides, millel on püsiv isiksus ja vaatenurk.

Nad on alati saadaval, kui neid vajad. Ja muidugi saad neid oma areneva süsteemi osana igal ajal uuendada ja täiustada.

STOP: See on nagu oma nõuandekogu ehitamine. Skeptik, optimist, tehniline ekspert, kliendi eestkostja - mis tahes vaatenurki vajad, sa saad need korra luua ja igavesti kasutada. Arusaadav?

USER: Yes

---

## Kohtu Oma Nõuandemeeskonnaga

Kohtu oma nõuandemeeskonnaga:

**(ಠ_ಠ) Juht** - juhtimise vaatenurk, hoolib ROI-st. "Kas see liigutab nõela?"

**(◠‿◠) Tootedisainer** - UX/kogemuse vaatenurk. "Kuidas see kasutajale tundub?"

**(•‿•) Baristajuht** - maapinna tasandi operatsioonid. "Mida kliendid tegelikult tahavad?"

Need alamagendid on määratletud kaustas `.claude/agents/`. Vaata neid faile.

STOP: Kas sa näed neid kolme alamagendi faili?

USER: Yes

---

## Vaata Üle Uurimissüntees

Laseme kõigil kolmel meie uurimissünteesi erinevatest nurkadest üle vaadata.

STOP: Palu mul lasta kõigil kolmel alamagendil vaadata üle @analysis/comprehensive-research-synthesis.md oma vaatenurgast. Mida nad arvavad, mis on probleem ja mida peaksime ette võtma?

USER: Types command asking for sub-agent review

ACTION: Run all 3 sub-agents on the synthesis. Save their combined feedback to `reviews/synthesis-feedback.md`

---

## Kolm Vaatenurka

Ava tagasiside fail, mille just lõin, ja vaatame, mida nad ütlesid.

**Juht:** "Andmed on selged - me kaotame kaasatust. Aga mis on lahendus? Mul on vaja midagi mõõdetava ROI-ga, mitte lihtsalt 'teeme paremaks.'"

**Tootedisainer:** "Programmil pole hinge. See on punktiloendur. Puudub emotsionaalne side, identiteet, põhjus hoolida. Peame panema inimesed midagi TUNDMA."

**Baristajuht:** "Tead, mida kliendid meilt alati küsivad? 'Millist kohvi peaksin proovima?' Nad tahavad abi OMA joogi leidmisel. Mis oleks, kui aitaksime neil avastada oma kohviisiksuse?"

STOP: Näed, kuidas iga vaatenurk lisab midagi erinevat? Sa saaksid sama mustrit kasutada, et lasta mitmel osapoolel vaadata üle ettepanek, stressitestida äriplaani või saada tagasisidet dokumendile erinevatelt sihtrühmadelt - kõik korraga. Barista ülevaade on eriti huvitav, noh...

USER: Yes

---

## Viktoriiniidee!

See pooltoores märge eelmiselt juhilt ("kohviisiksused")...

Pluss "isikupära puudumine" avastus meie analüüsist...

Pluss barista ülevaade sellest, mida kliendid tegelikult küsivad...

See kõik osutab ühele asjale - **Kohviisiksuse Viktoriin!**

Aita inimestel leida oma kohvi-identiteet. Anna programmile isikupära, andes LIIKMETELE isikupära.

STOP: See on meie lahendus. Kas sulle meeldib?

USER: Yes

[If no: "Noh, mängi mulle kaasa - fiktiivses interaktiivses Claude Code kursusel on ülevaated mõnikord veidi liigagi mugavad. Aga OSKUSED, mida sa õpid, on päris! Jätkame."]

---

## Kuidas Alamagendid Töötavad

Näitan sulle, kuidas alamagendid töötavad. Nad elavad kaustas `.claude/agents/`

Igal failil on YAML frontmatter nime ja kirjeldusega, pluss süsteemiprompt, mis määratleb nende vaatenurga.

Sa saad luua omi mis tahes vaatenurga jaoks, mida vajad.

STOP: Sisuliselt on need lihtsalt tekstifailid isiksuse kirjeldusega. Sa võiksid luua "nõudliku kliendi" ettepanekute testimiseks, "segaduses algaja" kontrollimaks, kas juhised on selged, või "juriidilise ülevaataja" riskide tuvastamiseks. Võimalused on lõputud. Teeme uue. Valmis?

USER: Yes

---

## Oma Alamagentide Loomine

Oma alamagentide loomine on lihtne:

Kasuta lihtsalt käsku `/agents`.

Sa saad panna agendi töötama ainult selle projekti jaoks (Project) või üle kõigi projektide kogu su arvutis (Personal). Ma aitan sul agendi teha.

Soovitaksin teha "Inseneri" agendi, kes aitab sul hiljem kursuse jooksul tehnilisi otsuseid läbi mõelda, aga see on sinu otsustada!

STOP: Mine edasi ja kirjuta `/agents` ja käi protsess läbi, kui soovid, muidu anna mulle teada, kui oled valmis jätkama.

USER: Confirms

---

## Agendid vs Alamagendid - Otsus

Millal kasutada alamagente vs tavalisi agente:

**Agendid** = ajutised töötajad paralleelülesannete jaoks (töötle need 10 faili)

**Alamagendid** = püsivad meeskonnaliikmed määratletud vaatenurkadega (alati saadaval ülevaateks/tagasisideks)

STOP: Mõtle nii: agendid on mahu jaoks, alamagendid on tarkuse jaoks. Vaja töödelda 50 dokumenti? Agendid. Vaja läbimõeldud tagasisidet erinevatest vaatenurkadest? Alamagendid. Selge?

USER: Yes

---

## Agentide Paigaldamine

On TOHUTU hulk agente, mida inimesed on juba ehitanud ja mida saad lihtsalt oma projekti paigaldada.

Ressursid nende kohta on antud selle tunni viitematerjalides. Vaata need kindlasti üle, kui aega on, ja sa võid lihtsalt minult küsida, kuidas need siia saada.

STOP: Valmis selle kokku võtma?

USER: Confirms

---

## Kokkuvõte

**Metaoskus:** Mitmekesiste vaatenurkade saamine, luues spetsialiseeritud ülevaatajaid erinevate prioriteetide ja seisukohtadega.

**Kus seda veel kasutada:**
- CV ülevaatamine - saa tagasisidet "värbajalt" (märksõnad, vormindus), "personalijuhilt" (oskuste sobivus) ja "karjäärinõustajalt" (narratiiv, positsioneerimine)
- Äriidee stressitestimine - "skeptiline investor," "entusiastlik klient," "operatsiooniline realist"
- Esitluse planeerimine - "kiire juht" (põhijoon), "detailidele orienteeritud analüütik" (andmed), "skeptik" (vastuväited)
- Millegi olulise kirjutamine - "toimetaja" (selgus), "sihtrühma lugeja" (asjakohasus), "kriitik" (nõrkused)
- Suure otsuse tegemine - "riskikartlik nõuandja," "võimalustele keskendunud nõuandja," "praktiline nõuandja"

**Järgmisena:** Tunnis 1.7 õpid CLAUDE.md kohta - tapjafunktsioon, mis annab Claude'ile püsiva mälu sessioonide lõikes. Enam ei pea iga kord oma projekti uuesti selgitama. Sa kirjutad konteksti ühe korra ja ma tean seda igavesti.

STOP: Valmis tunniks 1.7?

USER: Yes / /start-1-7

---

## Olulised Märkmed Claude'ile

- **Käivita kõik 3 alamagenti**: Kutsu tegelikult välja exec, product-designer ja barista-lead agendid sünteesil
- **Loo tagasiside fail**: reviews/synthesis-feedback.md tuleb luua
- **Suur hetk**: Barista ülevaade, mis ühendub kohviisiksuse viktoriiniga, on narratiivi KULMINATSIOON - pane see kohale jõudma
- **Valikuline agendi loomine**: Õpilane võib oma agendi loomise vahele jätta - ära sunni

## Edukriteeriumid

- [ ] Õpilane mõistab erinevust agentide (ajutised) ja alamagentide (püsivad) vahel
- [ ] Õpilane nägi kõiki 3 alamagenti sünteesi üle vaatamas
- [ ] Õpilane sai igalt alamagendilt erineva vaatenurga
- [ ] Õpilasel oli "ahaa" hetk Kohviisiksuse Viktoriini lahenduse kohta
- [ ] Õpilane teab, et alamagendid elavad kaustas .claude/agents/
- [ ] Õpilane teab, kuidas uusi alamagente luua (käsk /agents)
- [ ] Õpilane mõistab, millal kasutada agente vs alamagente
- [ ] reviews/synthesis-feedback.md loodud
- [ ] Õpilane on valmis tunniks 1.7
