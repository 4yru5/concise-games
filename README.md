# 0x Snake

A tiny, dependency-free Snake game: the snake is made of `0` characters and its food is `X`. Eat every available cell to clear the grid and win.

## Play

- Open **[Play 0x Snake](https://4yru5.github.io/concise-games/)** after GitHub Pages is enabled.
- Use **arrow keys** or **WASD** to steer.
- Press **Space** to pause and **R** to reset.
- On touchscreens, swipe the board or use the directional pad.
- Avoid walls and your own body. Each `X` eaten grows the snake.

## Offline

The game has no external libraries, fonts, images, APIs, or network calls. When served over HTTPS, its service worker caches the game shell so it can be played offline after the first successful visit. You can also download/clone the repository and open `index.html` directly; gameplay works without internet, though service-worker installation requires localhost or HTTPS.

## Run locally

Simply open `index.html` in a browser. To test service-worker offline caching, serve the folder locally:

```bash
python3 -m http.server 8000
```

Then visit http://localhost:8000.

## Deploy with GitHub Pages

In the repository settings, open **Pages**, choose **Deploy from a branch**, select `main` and `/(root)`, then save. After deployment, open the Pages URL once while online; subsequent visits can work offline.

## Built with

Plain HTML, CSS, Canvas, and JavaScript. No build step or dependencies.
