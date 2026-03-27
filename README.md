# Snowglobe

Consolidated blog repo for [zmackie.com](https://zmackie.com). This is the revival and unification of several blogs started over the years.

## Structure

```
content/
  posts/         - All blog posts (see history below)
  about.md       - About page
_archive/
  blogTheme/     - Ghost "Scriptor" theme from the pre-Hugo era (2015–2018)
```

## Blog History

This repo consolidates posts from several repos:

| Repo | Era | What it was |
|------|-----|-------------|
| `zmackie/blog` | 2016–2018 | Hugo blog (black-and-light theme), hosted at blog.zandermackie.com. Had ~30 converted posts stranded in `doc_conv/` that never made it to `content/post/`. |
| `zmackie/blogTheme` | 2015–2018 | Custom Ghost "Scriptor" theme — the platform before migrating to Hugo. Archived in `_archive/blogTheme/`. |
| `zmackie/zblog` | 2018–2021 | Hugo blog (PaperMod theme), deployed via Netlify. Security research, Go deep-dives, personal essays. This is the base for the current setup. |
| `zmackie/writing` | 2017 | Loose drafts: an OSS contribution guide and Elixir resource roundup (from a Stride newsletter). |
| `zmackie/zanadar.github.io` | 2016–2018 | Compiled HTML output of `zmackie/blog`, published to GitHub Pages. Not consolidated (it's generated output). |
| `zmackie/deep-thoughts` | 2023–2024 | Quarto-based blog ("Giant Morons"). Private repo — needs to be manually pulled in. Posts: weekly journals, AI/ML lesson writeups. |

## Post Eras

- **RC daily journals** (`02_08` – `03_15`): Daily logs from the [Recurse Center](https://recurse.com) Spring 1 2016 batch.
- **Early technical** (`XOR-for-distance`, `#each-in-Elixir`, `Go`, etc.): First technical deep-dives, 2016.
- **Personal essays** (`Limits`, `Night-&-Day`, `Important-Problems`): Reflections on programming, depression, and learning.
- **Security era** (`bug-bounties`, `flaws-writeup`, `h101ctf-*`, `warts-and-all-*`): Bug bounty writeups and CTF notes, 2020.
- **Go deep-dives** (`defer`, `functional-options`, `interface-pointer`): Go internals exploration, 2020.
- **Drafts** (`content/posts/_drafts/`): Unpublished pieces from the `writing` repo.

## Setup

This blog uses [Hugo](https://gohugo.io/) with the [PaperMod](https://github.com/adityatelange/hugo-PaperMod) theme and deploys via [Netlify](https://netlify.com).

```bash
# Install Hugo, then:
git submodule update --init --recursive
hugo server
```

## TODO: Pull in deep-thoughts

`zmackie/deep-thoughts` (the Quarto "Giant Morons" blog) is private and couldn't be cloned automatically. To bring it in:

```bash
git clone git@github.com:zmackie/deep-thoughts.git /tmp/deep-thoughts
cp -r /tmp/deep-thoughts/posts/* content/posts/_deep-thoughts/
```
