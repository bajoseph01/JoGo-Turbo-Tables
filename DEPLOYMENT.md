# Deployment Notes

## Current Status

The app is ready as a static GitHub Pages app:

- root entrypoint is `index.html`;
- all paths are relative;
- no external libraries are required;
- `manifest.webmanifest` is included;
- Apple Home Screen metadata and icons are included;
- iPad-sized touch testing passed locally.

## Current Blocker

GitHub Pages could not be enabled while this repository is private on the current GitHub plan.

Attempted command:

```powershell
gh api --method POST repos/bajoseph01/JoGo-Turbo-Tables/pages -f "source[branch]=main" -f "source[path]=/"
```

GitHub response:

```text
Your current plan does not support GitHub Pages for this repository.
```

## Decision Needed

To give learners a normal GitHub Pages link, choose one:

1. Make the repository public, then enable Pages from `main` and `/`.
2. Move the project to an account or organization plan that supports Pages for private repositories.
3. Host the static files elsewhere.

Do not make this repository public without Mr Jo's explicit permission.

## Expected Learner URL

Once Pages is enabled:

```text
https://bajoseph01.github.io/JoGo-Turbo-Tables/
```

## iPad Use

Open the Pages URL in Safari, then use Share -> Add to Home Screen.
