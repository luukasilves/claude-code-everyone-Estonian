# 2.4 GitHub

Praegu on su viktoriin ainult su arvutis.

Kui su sülearvuti lakkab töötamast või sa kustutad failid, on see kadunud. Ja me ei saa seda veel internetti panna.

Kõigepealt peame selle pilve salvestama. Selleks ongi GitHub.

STOP: Kas oled varem GitHub'i kasutanud?

USER: Yes / No / A little

---

GitHub on nagu Google Drive, aga koodi jaoks.

See salvestab su koodi pilve, hoiab iga muudatuse ajalugu ja laseb sul vigu tagasi võtta.

See on ka viis, kuidas me su viktoriini internetti saame – teenus, mida kasutame, peab su koodi kuskilt kätte saama.

Su projekti GitHub'is nimetatakse "repository'ks" (lühidalt "repo"). Sa kuuled arendajaid seda sõna palju kasutamas.

STOP: Selge?

USER: Yes

---

Kõigepealt on sul vaja GitHub'i kontot.

STOP: Kas sul on GitHub'i konto? Kui mitte, saan sulle registreerimislehe avada.

USER: I have one / Open it for me / I'll do it myself

ACTION: If they want it opened, run: `open https://github.com` (or bash open on Mac)

STOP: Anna mulle teada, kui sul on konto olemas ja oled valmis jätkama.

USER: Ready

---

Nüüd pean ma su GitHub'i kontoga ühenduse looma, et saaksin su koodi sinna salvestada.

Ma laadin alla mõned tööriistad, mis lasevad mul otse GitHub'iga töötada – nii et sa ei pea kunagi hirmutavaid käske tippima.

See võib avada su brauseri sisselogimiseks – lihtsalt järgi juhiseid ja tule tagasi, kui valmis.

ACTION: Set up GitHub CLI:

1. Check if already installed:
```
gh --version
```

2. If NOT installed:
   - On Mac: `brew install gh`
   - If brew fails or not on Mac: Tell user to go to https://cli.github.com and download manually, then come back

3. Once installed, authenticate (run in background to avoid blocking):
```bash
gh auth login --web --git-protocol https > /tmp/gh-auth.log 2>&1 &
sleep 2
cat /tmp/gh-auth.log
```

4. Read the output to get the one-time code, then open the device auth page:
```bash
open https://github.com/login/device
```

5. Tell user: "I just opened a page in your browser. Enter this code: [CODE FROM OUTPUT]. Click Authorize, then let me know when you're done."

STOP: Anna mulle teada, kui oled autoriseerinud.

USER: Done

ACTION: Verify authentication worked:
```bash
gh auth status
```

If successful, continue. If not authenticated, troubleshoot:
- They may not have completed the browser flow - ask them to try again
- The background process may have timed out - run the auth command again

---

Nüüd salvestame su koodi GitHub'i. Teen selle vaikimisi privaatseks, et ainult sina näeksid seda.

ACTION: Run the following commands in order:

1. Navigate to the quiz-project folder:
```
cd [path to quiz-project]
```

2. Initialize git (if not already done):
```
git init
```

3. Add all files:
```
git add .
```

4. Create initial commit:
```
git commit -m "Initial commit - coffee personality quiz"
```

5. Create GitHub repo and push:
```
gh repo create quiz-project --private --source=. --push
```

Valmis! Su kood on nüüd GitHub'is salvestatud. Arendajad nimetavad seda "push'imiseks" – sa push'id oma koodi pilve.

Avan selle sulle, et sa saaksid vaadata.

ACTION: Get the repo URL and open it:
```
gh repo view --web
```
(This opens the GitHub repo in your browser)

STOP: Kas sa näed oma projekti GitHub'is?

USER: Yes!

---

Su viktoriin on nüüd varundatud ja valmis ellu minema.

Nüüdsest, kui tahad oma tööd salvestada, palu mul lihtsalt "push'i GitHub'i" ja ma salvestan su viimased muudatused.

GitHub'il on palju rohkem võimalusi – koostöö, versiooniajalugu, harud – ja tulevikus tuleb sellest eraldi moodul. Aga praegu on oluline see: su kood elab kohas, kust sellele saab ligi, et see internetti panna.

Täpselt seda me järgmisena teemegi.

**Järgmisena:** Tunnis 2.5 paneme su viktoriini internetti! Me ühendame GitHub'i teenusega nimega Vercel ja sa saad päris URL-i, mida saad kellelegi jagada. See on finišijoon.

STOP: Valmis ellu minema? Ütle "lähme" või kirjuta /start-2-5

USER: Let's go

---

## Olulised märkmed Claude'ile

- GitHub CLI (gh) on kõige lihtsam viis autentimiseks – ära palu kasutajatel SSH võtmeid seadistada
- Lipp `--private` on oluline – kasutajad ei taha, et nende viktoriini kood oleks vaikimisi avalik
- Kui neil on juba repo nimega quiz-project, gh annab vea – aita neil valida teine nimi
- Käsk `gh repo view --web` on palju puhtam kui URL-i ise kokku panna
- Kui brew pole saadaval, on cli.github.com-is paigaldajad kõigile platvormidele
- Next.js projektidel on juba .gitignore, nii et node_modules'it ei commit'ita

## Edukriteeriumid

- Kasutajal on GitHub'i konto
- GitHub CLI on paigaldatud ja autenditud
- Kood on commit'itud ja push'itud privaatsesse GitHub'i repository'sse
- Kasutaja näeb oma repot github.com-is
- Kasutaja saab aru, et saab paluda "push'i GitHub'i" tulevaste muudatuste salvestamiseks
