# Qino CMS

**A modern, Deno-native CMS for editing websites where they live.**

Qino CMS combines direct inline editing with a compact, modular architecture. Content editors get a natural editing experience, while developers keep full control over layouts, content types, permissions, and integrations.

- Inline editing directly on the website
- Extensible content, layout, backend, and integration modules
- Built-in authentication and WebAuthn support
- Analytics and MCP integration
- TypeScript, ESM, and Web-standard APIs
- Powered by the lightweight [Qino application core](https://github.com/qinojs/qino)

## Try the editor in your browser

[Open the interactive Qino CMS demo](https://schwups.ch/qino#ausprobieren). The demo page is in German. You can edit sample content directly on the page and reset it without creating an account.

Qino CMS is developed by [schwups GmbH](https://schwups.ch/).

## Quick start

Clone Qino and enter the repository:

```sh
git clone https://github.com/qinojs/qino.git
cd qino
```

Create a `server.ts`:

```ts
import { App } from "./module/core/mod.ts";

const app = new App({
  db: `sqlite:${import.meta.dirname}/site.sqlite`,
  dev: true,
});

app.stores
  .add(new URL("./module/store.json", import.meta.url))
  .add("cms")
  .add("cms.installation.default");

await app.init();

Deno.serve({ port: 8000 }, app.fetch);
```

Start the site:

```sh
deno run -A server.ts
```

Open [http://localhost:8000](http://localhost:8000). On the first start, Qino creates the CMS structure and prints the generated superuser credentials in the terminal.

## Repository status

This repository is currently a placeholder. The CMS source still lives alongside the Qino core in the [qinojs/qino](https://github.com/qinojs/qino) repository.

## License

[MIT](LICENSE)
