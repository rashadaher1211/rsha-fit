RSHA FIT V2
===========

WHAT IS NEW
- Rebranded from PinkFit to RSHA FIT
- Installable PWA setup for iPhone home screen
- App icons
- Favorites
- Recently used exercises
- Rest timer (1:00 / 1:30 / 2:00 / 3:00)
- Automatic rest timer after completing a set
- Workout history with workout details
- Progress page
- Total training volume
- Personal bests
- Top exercises by volume
- Starter library with 46 exercises
- Online-sync button prepared for wger public exercise data
- Image/video fields and video-search fallback
- Offline cache after the online app has been opened once

HOW TO TEST ON WINDOWS
1. Open index.html.
2. The main local features work immediately.
3. Some browser security rules can block the online exercise API when opening from file://.
   That is expected. The Sync button is meant for the hosted HTTPS version.

FREE INTERNET PUBLISHING WITH GITHUB PAGES
1. Create/sign in to a GitHub account.
2. Create a new PUBLIC repository named: rsha-fit
3. Upload ALL files from this folder to the root of the repository.
4. Open repository Settings -> Pages.
5. Under Build and deployment, choose "Deploy from a branch".
6. Branch: main. Folder: /(root). Save.
7. GitHub will provide a URL similar to:
   https://YOUR-USERNAME.github.io/rsha-fit/
8. Open that URL in Safari on your iPhone.
9. Safari -> Share -> Add to Home Screen -> Add.
10. RSHA FIT will appear as an app icon.

IMPORTANT ABOUT APPLE WATCH
The PWA can be installed on the iPhone but browsers do not get direct HealthKit/Apple Watch workout access.
A real Apple Watch connection requires a native iOS/watchOS component using Apple's HealthKit APIs.
We can build that as a later phase, but signing/installing a watchOS app ultimately requires Apple development tooling and provisioning.

DATA
Workout history is currently stored in the browser/device using localStorage.
Do not clear Safari/site data if you want to keep this history.
A later upgrade can add export/import or cloud sync.
