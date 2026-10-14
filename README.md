# Traditional Artist Portfolio

## Deploy to GitHub Pages

This is a static website; no build step is required. The included GitHub Actions workflow publishes `index.html` to GitHub Pages whenever a change is pushed to `main`.

1. Push this project to a GitHub repository. If its default branch is not `main`, update the branch name in `.github/workflows/deploy.yml`.
2. In the repository, open **Settings → Pages** and set **Build and deployment → Source** to **GitHub Actions**.
3. Push a change to `main`, or start **Deploy to GitHub Pages** manually from the repository’s **Actions** tab.
4. When the workflow succeeds, open the Pages URL shown in the workflow run or in **Settings → Pages**.

The page is served from the repository root, so keep `index.html` there.

## Before publishing

- The page loads its fonts from Google Fonts, so those fonts require an internet connection. System font fallbacks are included.
- Artwork management is available without login. New artworks are saved only in the current browser's local storage; they are not shared across visitors or devices and can be cleared by the browser. A shared portfolio needs a database and image storage service.
