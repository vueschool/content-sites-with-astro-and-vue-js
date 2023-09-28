# Content Sites with Astro and Vue.js

![https://vueschool.io/courses/content-sites-with-astro-and-vue-js](https://vueschool.io/storage/media/fbedcf3f068608ef41fac94cae9da466/astro-vue.jpg)

This repository contains the example code for the [Content Sites with Astro and Vue.js](https://vueschool.io/courses/content-sites-with-astro-and-vue-js) course.

Combining Vue.js with Astro for building content sites, like blogs or docs, makes for a blazing-fast site and an A+ developer experience. Why? Astro is a modern front-end framework that allows you to build with the JavaScript technology of your choice (think React, Vue, Svelte, and more) but doesn’t ship any JavaScript by default. This is known as an islands architecture, where we opt-in to JavaScript instead of vice-versa.

In this course, learn the basics of getting started with Astro by building a simple blog. Also, learn to integrate it with your favorite JavaScript framework Vue.js for templating that’s familiar and for sprinkling in interactivity only where required.

[Enroll at Vue School](https://vueschool.io/register) to watch this course!

## 🚀 Project Structure

Inside of your Astro project, you'll see the following folders and files:

```text
├── public/
├── src/
│   ├── components/
│   ├── content/
│   ├── layouts/
│   └── pages/
├── astro.config.mjs
├── README.md
├── package.json
└── tsconfig.json
```

Astro looks for `.astro` or `.md` files in the `src/pages/` directory. Each page is exposed as a route based on its file name.

There's nothing special about `src/components/`, but that's where we like to put any Astro/React/Vue/Svelte/Preact components.

The `src/content/` directory contains "collections" of related Markdown and MDX documents. Use `getCollection()` to retrieve posts from `src/content/blog/`, and type-check your frontmatter using an optional schema. See [Astro's Content Collections docs](https://docs.astro.build/en/guides/content-collections/) to learn more.

Any static assets, like images, can be placed in the `public/` directory.

## 🧞 Commands

All commands are run from the root of the project, from a terminal:

| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Installs dependencies                            |
| `npm run dev`             | Starts local dev server at `localhost:4321`      |
| `npm run build`           | Build your production site to `./dist/`          |
| `npm run preview`         | Preview your build locally, before deploying     |
| `npm run astro ...`       | Run CLI commands like `astro add`, `astro check` |
| `npm run astro -- --help` | Get help using the Astro CLI                     |

## 👀 Want to learn more?

Check out [our documentation](https://docs.astro.build) or jump into our [Discord server](https://astro.build/chat).

## Credit

This codebase is based on the [Official Blog Theme from Astro](https://astro.build/themes/details/blog/)
