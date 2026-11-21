# Curing the Heart

Companion app for Ibn al-Qayyim's *Ad-Dā' wa ad-Dawā'* (The Disease and the Cure):

- **Today**: the times when du'a is answered, calculated from your prayer times, plus the Jumuʿah checklist
- **Prayers**: daily ticks for the five prayers on time, Jumuʿah, the 12 rakʿahs of Sunnah, Witr, 4 rakʿahs before sleep and qiyām al-layl, with a 7-day grid and streaks
- **Muḥāsabah**: a one-minute check of the four doors (glance, thought, word, step) after every prayer and before sleep
- **My du'as**: your own du'a list, tagged with the best moment for each
- **How to ask**: the etiquette of du'a from the book

Data is stored per user in Firestore under `users/{uid}/entries`. Only the signed-in owner can read it (see `firestore.rules`).

## Setup
1. Firebase console → create project → add **Web app** → copy the config into `firebase-config.js`.
2. **Authentication** → Sign-in method → enable **Google**.
3. Authentication → Settings → **Authorized domains** → add `athleticconsumer-dotcom.github.io`.
4. **Firestore Database** → create in **production mode** → Rules tab → paste `firestore.rules` → Publish.
5. GitHub repo → Settings → **Pages** → Deploy from branch `main`, folder `/ (root)`.
6. Open `https://athleticconsumer-dotcom.github.io/curing-the-heart/`, sign in with Google, done.

## Moving data from the Claude version
Claude version → Settings → **Copy my data**. GitHub version → sign in → Settings → paste into "Bring over data" → **Import**.

## App
Installable (PWA): Android Chrome menu → Install app. iPhone: Safari → Share → Add to Home Screen.
