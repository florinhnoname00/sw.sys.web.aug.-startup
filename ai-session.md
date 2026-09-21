# AI Session Notes

## Project

Web AR Three.js demo for aligning interactive 3D models with blue reference frames.

## Current behavior

- `index.html` is the main GitHub Pages entry point.
- The motorcycle helmet is loaded from `resources/casca_moto.glb`.
- The LEGO model is loaded from `resources/LEGO_1.glb`.
- Both models can be selected and moved by dragging.
- `M` or the `Rotire` button rotates around the Y axis.
- `N` or the vertical `Rotire` button rotates around the X axis.
- The camera and scene remain fixed while objects are manipulated.
- Reference frames use model-shaped outlines where available.
- The matching frame changes from blue to green when the selected object is within tolerance.
- Helmet alignment tolerance is 10%; LEGO alignment tolerance is 12%.

## Run locally

The project is served at:

```text
http://localhost:8000/index.html
```

The local server is a PowerShell `HttpListener` because Python is not available on this machine. If it is not running, start a local HTTP server that serves the project root on port 8000.

## Git workflow

Check changes:

```powershell
git status
git diff
```

Save the current session notes and code:

```powershell
git add -A
git commit -m "Describe the change"
```

Push the current branch to GitHub:

```powershell
git push origin HEAD
```

## Deployment

GitHub Pages repository:

```text
https://github.com/florinhnoname00/sw.sys.web.aug.-startup
```

Published site:

```text
https://florinhnoname00.github.io/sw.sys.web.aug.-startup/
```

GitHub Pages should use branch `main` and folder `/ (root)`. Upload or push `index.html`, the `resources/` folder, and this `ai-session.md` file before testing the public URL.

## Resume checklist

1. Open `ai-session.md` and `index.html`.
2. Run `git status`.
3. Start or verify the local HTTP server.
4. Open `http://localhost:8000/index.html`.
5. Test both models, their frames, touch buttons, tolerance behavior, and portrait layout.
6. Commit and push changes when ready.
