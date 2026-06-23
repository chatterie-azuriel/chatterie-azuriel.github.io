# Chatterie d'Azuriel — site web 🐾

The website for **Chatterie d'Azuriel**, a small family-run **Ragdoll cattery** in Strasbourg (Alsace, France). It's a single-page site, in French, that introduces the cats, shows the kittens currently available, and answers the questions people most often ask before adopting.

- 🌐 **Live site:** https://chatterie-azuriel.github.io/
- 💻 **Repository:** https://github.com/chatterie-azuriel/chatterie-azuriel.github.io
- 📸 **Instagram:** [@theodred_the_cat](https://www.instagram.com/theodred_the_cat/)
- 🏷️ **Annonce Leboncoin:** [voir l'annonce](https://www.leboncoin.fr/ad/animaux/3212185891)

## What's in here

| File | What it is |
|------|------------|
| **`index.html`** | The whole website — HTML **and** CSS are in this single file. No build step. |
| `logo_png.png` / `logo_cat_only.png` / `logo.jpg` | The logos (full lockup, cat-only mark, and a white-background version). |
| `mother_cat.jpg` · `father_cat.jpg` · `chat_2.jpg` | Photos of Yuzu (mum), Yumi (dad) and Theodred. |
| `violet.jpg` · `orange.jpg` · `rose.jpg` · `gris.jpg` · `bleu.jpg` | The five kittens. |
| `faq.md` | The full FAQ text (also embedded in `index.html`). |

## How to preview it

Just **double-click `index.html`** — it opens in any web browser. Nothing to install.

## How to edit the content

Open `index.html` in a text editor (VS Code, etc.). It's plain HTML, organised in clearly-labelled sections:

- `<!-- LE RAGDOLL -->` · `<!-- NOS CHATS -->` · `<!-- LES CHATONS -->` · `<!-- FAQ -->` · `<!-- CONTACT -->`

Common edits:
- **Change wording** → find the section and edit the text between the tags.
- **Mark a kitten as reserved** → in the `<!-- LES CHATONS -->` section, change that kitten's `<span class="badge">Disponible</span>` to `Réservé`.
- **Swap a photo** → replace the image file with one of the same name (e.g. overwrite `rose.jpg`), or change the `src="..."`.

### Pricing & availability
To change a price, the deposit, or a kitten's status (`Disponible` / `Réservé`), edit the relevant block in `index.html`. There are no unfinished placeholders left on the page.

## Hosting on GitHub Pages

This repo lives in the **`chatterie-azuriel`** organization and is named `chatterie-azuriel.github.io`, so GitHub Pages publishes it at the root domain **https://chatterie-azuriel.github.io/**.

To enable (or check) it:
1. **Settings → Pages**
2. *Build and deployment* → **Source: Deploy from a branch** → **Branch: `main`**, folder **`/ (root)`** → **Save**.
3. Wait ~1–2 minutes (the first publish can take a few); the live URL appears at the top of that same page.

Every push to `main` redeploys the site automatically.

## Tech notes

Static site, no framework and no build. Single `index.html` with inline CSS. Typography is **Geist** + **Geist Mono** (Google Fonts); the soft moving header is a CSS "aurora" gradient. Fully responsive and respects the user's *reduce motion* setting.

---
Made with ❤️ for our Ragdolls.
