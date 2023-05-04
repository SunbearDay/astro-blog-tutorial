# Astro Starter Kit: Minimal

```
npm create astro@latest -- --template minimal
```

[![Open in StackBlitz](https://developer.stackblitz.com/img/open_in_stackblitz.svg)](https://stackblitz.com/github/withastro/astro/tree/latest/examples/minimal)
[![Open with CodeSandbox](https://assets.codesandbox.io/github/button-edit-lime.svg)](https://codesandbox.io/p/sandbox/github/withastro/astro/tree/latest/examples/minimal)
[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/withastro/astro?devcontainer_path=.devcontainer/minimal/devcontainer.json)

> 🧑‍🚀 **Seasoned astronaut?** Delete this file. Have fun!

## 🚀 Project Structure

Inside of your Astro project, you'll see the following folders and files:

```
/
├── public/
├── src/
│   └── pages/
│       └── index.astro
└── package.json
```

Astro looks for `.astro` or `.md` files in the `src/pages/` directory. Each page is exposed as a route based on its file name.

There's nothing special about `src/components/`, but that's where we like to put any Astro/React/Vue/Svelte/Preact components.

Any static assets, like images, can be placed in the `public/` directory.

## 🧞 Commands

All commands are run from the root of the project, from a terminal:

| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Installs dependencies                            |
| `npm run dev`             | Starts local dev server at `localhost:3000`      |
| `npm run build`           | Build your production site to `./dist/`          |
| `npm run preview`         | Preview your build locally, before deploying     |
| `npm run astro ...`       | Run CLI commands like `astro add`, `astro check` |
| `npm run astro -- --help` | Get help using the Astro CLI                     |

## 👀 Want to learn more?

Feel free to check [our documentation](https://docs.astro.build) or jump into our [Discord server](https://astro.build/chat).

## Interesting Links

[YAML front matter](https://assemble.io/docs/YAML-front-matter.html)

[Markdown Cheat Sheet](https://www.markdownguide.org/cheat-sheet/)

[CSS Variables in Astro](https://docs.astro.build/en/guides/styling/#css-variables)

[Refactoring Article](https://refactoring.com/)

[Component Base Design Article](https://www.droptica.com/blog/component-based-design/)

[Semantic HTML Tags Article](https://www.dofactory.com/html/semantics)

[Mobile First Design Article](https://www.mobileapps.com/blog/mobile-first-design)

[Client-Side Scripts in Astro](https://docs.astro.build/en/guides/client-side-scripts/)

[Astro Layout Components](https://docs.astro.build/en/core-concepts/layouts/)

[Markdown Layouts in Astro](https://docs.astro.build/en/guides/markdown-content/#frontmatter-layout)

[Markdown Layout Props](https://docs.astro.build/en/core-concepts/layouts/#markdown-layout-props)

[Introduction to YAML](https://dev.to/paulasantamaria/introduction-to-yaml-125f)

[Nesting Layouts in Astro](https://docs.astro.build/en/core-concepts/layouts/#nesting-layouts)

## Add global styles to `.astro` file

Import the stylesheet into the frontmatter of the `.astro` file.

```yaml
---
import '../styles/global.css'
---
```

## Component Props

```js
---
// Usage: <GreetingHeadline greeting="Howdy" name="Partner" />
const { greeting, name } = Astro.props;
---
<h2>{greeting}, {name}!</h2>
```

We can also define a Props interface when using TypeScript.

```js
---
interface Props {
  name: string;
  greeting?: string;
}
const { greeting, name } = Astro.props;
---
<h2>{greeting}, {name}!</h2>
```
