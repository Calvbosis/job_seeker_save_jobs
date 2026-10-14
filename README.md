# Job seeker save jobs

Prototype and dev notes for the save heart animation on job seeker job cards.

## View it

Open `index.html` in a browser, or view it live on GitHub Pages:
https://calvbosis.github.io/job_seeker_save_jobs/

The page shows the job card in a phone frame. Tap the heart to save and unsave. The dev notes below the phone cover markup, animation specs, CSS, Angular component logic, colours and a build checklist.

## Summary

- **Save:** heart fills red (#BA1A1A) and pops, a faint ring ripples out and 6 dots burst away (about 420ms). Snackbar shows "Job saved".
- **Unsave:** heart returns to the grey outline with a small settle. Snackbar shows "Removed from saved jobs".
- **Hover:** 40px circle state layer behind the heart, grey when unsaved and red when saved.
- CSS keyframes only, no animation library. Snackbar uses Angular Material `MatSnackBar` with a 4 second duration.
- All animation turns off under `prefers-reduced-motion`.
