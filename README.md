# Roar

Static [Hugo](https://gohugo.io/) website using the [Blowfish](https://blowfish.page/) theme, deployed to GitHub Pages at <https://esl-epfl.github.io/roar/>.

## Local development

```bash
git submodule update --init --recursive
cd website/themes/blowfish && npm ci && cd -
cd website
mkdir -p assets/css/compiled
npx @tailwindcss/cli \
  -c ./themes/blowfish/tailwind.config.js \
  -i ./themes/blowfish/assets/css/main.css \
  -o ./assets/css/compiled/main.css --jit
hugo serve
```

Then open <http://localhost:1313/roar/>.

## Deployment

Pushes to `main` that touch `website/**` trigger the `Build website` workflow (`.github/workflows/2-build-website.yml`), which builds the site and publishes it to GitHub Pages.
