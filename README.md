# qdc-docs

بسم الله الرحمن الرحيم

This is the QDC documentation boilerplate, it's based on [VueJs](https://vuejs.org) framework, combined with @nuxt/content as its backbone.

For detailed explanation on how things work, checkout [nuxt/content](https://content.nuxtjs.org) and [@nuxt/content theme docs](https://content.nuxtjs.org/themes-docs).

In a nutshell, using @nuxt/content gives us a lot of highly valuable features for the QDC documentation, including (from [Nuxt's documentation](https://content.nuxtjs.org/#features)):

- Blazing fast hot reload in development
- Vue components in Markdown
- Full-text search
- Support static site generation with `nuxt generate`
- Powerful QueryBuilder API (MongoDB like)
- Syntax highlighting to code blocks in markdown files using PrismJS.
- Table of contents generation
- Handles Markdown, CSV, YAML, JSON(5), XML
- Extend with custom parsers
- Extend with hooks
  and Light and dark mode.

This boilerplate is very robust that it's used by Nuxt itself along with a lot of other big projects like [Hoppscotch](https://docs.hoppscotch.io/).

## Community

This API has a very active and helpful community where you can discuss, get help or share your ideas!
[Join Quran.com Discord community »](https://discord.gg/SpEeJ5bWEQ)

## Setup

Install dependencies:

```bash
npm run install
```

## Development

```bash
npm run dev
```

## Static Generation

This will create the `dist/` directory for publishing to static hosting:

```bash
npm run generate
```

To preview the static generated app, run `npm run start`
