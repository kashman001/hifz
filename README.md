# Hifz Tracker — stable link

A one-file redirect: `https://kashman001.github.io/hifz/` is the **permanent bookmark** for the
Hifz Tracker web app. It forwards to the app's current Google Apps Script `/exec` URL, preserving
the query string (`?s=<link key>`).

Why: Apps Script caps a script at 200 lifetime versions, so the app's `/exec` URL must eventually
rotate. This page is the layer that keeps everyone's bookmarks working — a rotation is a one-line
edit to `TARGET` in `index.html`.

No data is stored here. The student link key travels only in the URL the student already has;
prefer the `#s=<key>` fragment form if you want it kept out of request logs.

The tracker itself: [Quran_Hifz_Tracker](https://github.com/kashman001/Quran_Hifz_Tracker).

## docs/
The product documentation (user guide, architecture, …) served at
https://kashman001.github.io/hifz/docs/. **Generated** from the tracker repo's `docs/product/`
by `npm run publish-docs` — don't edit here; changes belong in the tracker repo.
