# Italia Personal Finance Wiki - Reddit

# 👋 Intro in Italiano

Wiki open source del progetto Italia Personal Finance.

Di seguito le istruzioni per aggiungere o modificare un contenuto anche se non avvezzi a GitHub.

In caso di problemi aprite una "issue" dal menu apposito e cercheremo di aiutarvi.

## 📋 To-Do List

### ✨ Idee da realizzare

- file excel di esempio per budgeting e tracking investimenti

- Approfondimento [tassazione](src/content/blog/taxation.mdx)

- Differenza tra redditi da capitali e diversi

### 💼 In corso di realizzazione

- Theme switcher

- Arricchimento pagina articoli esistenti (open to ideas)

## 🔨 Vuoi contribuire scrivendo o modificando un articolo?

Puoi farlo direttamente anche da GitHub, tutti gli articoli sono nella cartella `src/content/blog` e sono in markdown,
la stessa sintassi usata su Reddit (`.md` e `.mdx`).

![Tutorial video](https://github.com/emish89/italiapersonalfinance/blob/main/readme/pr-gif.gif)

### Step 1

Vai nella cartella `src/content/data/blog` e seleziona l'articolo da modificare o premi "add file" in alto a destra

### Step 2

Premi "Fork this repository", andando quindi a creare la versione del repository forkata nel tuo profilo

### Step 3

Modifica il contenuto come preferisci e alla fine premi "Commit changes" in alto a destra

### Step 4

Aggiungi un "commit message" che spieghi cosa hai aggiunto o modificato brevemente

### Step 5

Premi "propose change"

### Step 6

Aggiungi un titolo e una descrizione alla pull request, che permetta di capire cosa stai andando ad aggiungere/modificare

### Step 7

Nella schermata successiva premi "create pull request" in alto a destra

### Step 8

Attendi che uno dei maintainer approvi la richiesta e a quel punto il tuo contenuto verrà pubblicato!

## 🍼 Vuoi contribuire in modo più semplice?

Se non hai familiarità con GitHub e vuoi contribuire alla wiki oppure se esiste già un post su Reddit e vuoi segnalarlo per farlo aggiungere,
puoi utilizzare questi 2 semplicissimi metodi:

- [Clicca qui per aggiungere un articolo](https://github.com/emish89/italiapersonalfinance/issues/new?assignees=emish89&labels=article&projects=&template=new_article.md&title=)

- [Clicca qui per segnalare un post da aggiungere](https://github.com/emish89/italiapersonalfinance/issues/new?assignees=emish89&labels=post&projects=&template=post_to_article.md&title=)

# 🪒 Technical part

## Articles

All the wiki articles are in the `src/content/blog` folder, they are markdown (`.md` and `.mdx`) files.
You can create a PR for adding new articles or change the content of the existing ones only playing with markdown.
No other knowledge needed

## Usage

This project is based on [Astro Framework](https://github.com/withastro/astro) with [UnoCSS](https://uno.antfu.me/) and [Brutal theme](https://github.com/ElianCodes/brutal)

### Commands

All commands are run from the root of the project, from a terminal:

(Here I use NPM, no problem if you use PNPM or Yarn)

| Command                 | Action                                             |
| :---------------------- | :------------------------------------------------- |
| `npm install`           | Installs dependencies                              |
| `npm run dev`           | Starts local dev server at `localhost:3000`        |
| `npm run build`         | Build your production site to `./dist/`            |
| `npm run preview`       | Preview your build locally, before deploying       |
| `npm run astro ...`     | Run CLI commands like `astro add`, `astro preview` |
| `npm run astro --help`  | Get help using the Astro CLI                       |

## Integrations

###

In this project, I'm using [UnoCSS](https://uno.antfu.me/) to generate the CSS. It's a utility-first CSS framework that uses a single class to style elements. It's very easy to use and has a lot of features. It's setup to be completely compatible with TailwindCSS, with the advantage of being able to use PureCSS icons. You can always switch out UnoCSS for TailwindCSS if you want to, without breaking the general styles.

### Sitemap

To generate the sitemap, you don't need to do anything. It's automatically generated when you build your site. You'll just need to switch out the `site` on `astro.config.mjs` to your own.

```js title="astro.config.mjs"
import { defineConfig } from 'astro/config';

export default defineConfig({
  site: 'https://example.com',
});
```

### RSS

The RSS feed is automatically generated from the Markdown files in the `src/content/blog` folder.

The RSS will output to `https://example.com/feed.xml` by default. Can be changed by renaming `src/pages/feed.xml.js`.

## Components

### `components/blog/`

This directory contains all components for the blog.

### `components/errors/`

This directory contains all error components.

#### `components/errors/404.astro`

This component is used when a page is not found.

### `components/generic/`

This directory contains all generic components, reused over multiple pages.

### `components/home/`

This directory contains all components for the home page.

### `components/layout/`

This directory contains all layout components. For instance, the header and footer and `<head>` section.

## Suggestions

All the suggestions in terms of wiki content are really appreciated. You can create a PR with the markdown file or write us the content in a proper feature request.

## 🚶 Disclaimer

The information provided on this wiki is for general informational purposes only. It is not intended as, and should not be considered, financial advice. We strongly recommend that you consult with a qualified financial advisor or professional before making any financial decisions.

Accuracy and Completeness:
While we strive to provide accurate and up-to-date information, this wiki makes no representations or warranties of any kind, express or implied, about the completeness, accuracy, reliability, suitability, or availability with respect to the information provided. Any reliance you place on such information is therefore strictly at your own risk.

Investment Risks:
Investing in financial markets involves risk, and past performance is not indicative of future results. The value of investments may fluctuate, and investors may lose their entire investment. The wiki is not responsible for any financial loss or damage that may arise from your use of the information provided.

If you have any questions about this disclaimer or the information on this wiki, please contact us through GitHub.


![Alt](https://repobeats.axiom.co/api/embed/5d01a4e83f2626e1beb0b9d7c0331daf224e13b0.svg "Repobeats analytics image")
