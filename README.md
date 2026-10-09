# Workout Chooser

A small web app for building a circuit workout from the exercises you know. Pick how many groups you have time for and how many upper body, lower body and core exercises you want. The app splits them into groups of about three, shows the weight and reps you used last time, and logs what you did after each group.

It puts the exercises you haven't done for the longest time first, so you rotate through everything instead of repeating the same few.

## Using it on your phone

Open the site in your phone's browser, then:

- **iPhone (Safari):** tap Share, then **Add to Home Screen**.
- **Android (Chrome):** tap the menu, then **Install app** or **Add to Home screen**.

It opens like a normal app and works without a signal once it has been opened once.

## Where your data is saved

Everything is saved in the browser on the device you use. Each phone or computer keeps its own list, and clearing the browser's site data erases it. Use **History → Backup → Export my data** now and then to keep a copy, and **Import a backup** to restore it or move it to another device. Importing merges with what's already there: exercises match by name and log entries are only added once.

## Files

- `index.html` is the whole app: markup, styles and script.
- `sw.js` keeps the app available offline. Change `CACHE` in it whenever you edit the app so installed copies pick up the update.
- `manifest.webmanifest` and `icons/` make it installable.

There is no build step. To try it locally, run `python3 -m http.server` in this folder and open http://localhost:8000.
