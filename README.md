# StrongLifts 5×5 Tracker

This is a small installable Progressive Web App (PWA) for Android.

## Your starting state

- Next workout: Workout B
- Training days: Monday / Wednesday / Friday
- Workout A completed on 24 August 2026
- Squat: 20 kg completed → next target 22.5 kg
- Bench press: 40 kg completed → next Workout A target 42.5 kg
- Barbell row: 40 kg completed → next Workout A target 42.5 kg
- Workout B starting weights are provisional until edited in Setup

## Programme

Workout A:
- Squat 5×5
- Bench press 5×5
- Barbell row 5×5
- Pull-up 3×8
- Hanging knee raises 3×8

Workout B:
- Squat 5×5
- Overhead press 5×5
- Deadlift 1×5
- Barbell curl 3×8
- Plank 3×30 sec

## Progression logic

- Successful prescribed sets/reps: add the configured increment next time.
- Miss any rep: repeat that weight.
- Three unsuccessful attempts at a weight: deload 10%, rounded to the nearest 2.5 kg.
- Default increments: 2.5 kg for most lifts, 5 kg for deadlift.
- These values can be edited in Setup.

## Put it online with GitHub Pages

1. Create a free GitHub account if you do not already have one.
2. Create a new repository, e.g. `stronglifts-tracker`.
3. Upload ALL files from this folder into the root of that repository.
4. In the repository, open **Settings → Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**.
6. Select the `main` branch and `/ (root)` folder, then save.
7. GitHub will give you a public HTTPS URL after deployment.

Then on Android:
1. Open that URL in Chrome.
2. Tap the install prompt inside the app, or Chrome's ⋮ menu.
3. Choose **Install app** or **Add to Home screen**.
4. The StrongLifts icon will appear on your home screen.

## Data storage

Workout data is stored locally on that device in browser storage. It persists between app launches and works offline after the first visit. Clearing the site's browser data will erase the workout history.

## Current limitation

Reliable scheduled Android workout notifications are not included in this version. That would require either a push-notification backend or converting the tracker into a native Android app.
