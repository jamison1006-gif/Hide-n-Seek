# Hide & Seek — Moonlight Garden

A browser-based 3D hide-and-seek game built with Three.js and Vite.

## Open as a link

Once published, players simply open the website and click **Play now**. No installation or account is needed. **Copy game link** copies the published address for sharing.

### Publish with GitHub Pages

1. Push these project files to the `main` branch of `jamison1006-gif/Hide-n-Seek`.
2. In the repository, open **Settings → Pages → Build and deployment** and select **GitHub Actions** as the source.
3. Open **Actions → Publish game to GitHub Pages** and run the workflow (or push to `main`).
4. Use the website link shown by the completed deployment. The expected address is `https://jamison1006-gif.github.io/Hide-n-Seek/`; it is only live after a successful deployment.

The included workflow builds and publishes `dist/` automatically on future pushes to `main`. If Pages is unavailable for this repository, enable Pages for its visibility/plan or use another static host with build command `npm run build` and output directory `dist`.

## Run

Requires Node.js 20.19+ or 22.12+.

```sh
npm ci --cache /tmp/hide-seek-npm-cache
npm run dev
```

Build with `npm run build`; serve the production build with `npm run preview`.

## Play

- Click **Play now** to start a round.
- Move with WASD or the arrow keys. Drag to orbit; scroll to zoom.
- Get close to a glowing wardrobe, crate, barrel, or bush and click it to hide.
- The character disappears inside; the third-person camera remains outside.
- Press **E** to leave your spot.
- You have 15 seconds to hide, then must survive a 60-second search.
- The NPC follows paths around obstacles, spots exposed players in its forward field of view, chases them, and inspects hiding spots in a randomized order.
- **New round** restarts immediately.

Desktop keyboard and mouse recommended. No backend or credentials required. Fonts optionally load from Google Fonts, with local fallbacks.
