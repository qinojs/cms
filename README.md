# Qino CMS

**A TypeScript CMS for editing websites in place.**

Qino CMS combines direct inline editing with a compact, modular architecture. Content editors get a natural editing experience, while developers keep full control over layouts, content types, permissions, and integrations.

- Inline editing directly on the website
- Extensible content, layout, backend, and integration modules
- Built-in authentication and WebAuthn support
- Analytics and MCP integration
- TypeScript, ESM, and Web-standard APIs
- Powered by the lightweight [Qino application core](https://github.com/qinojs/qino)

## About Qino CMS

[Qino CMS product information](https://schwups.ch/qino) is available in German.

Qino CMS is developed by [schwups GmbH](https://schwups.ch/). The CMS ships with the Qino framework as the `/cms` subpath of [`qinojs` on npm](https://www.npmjs.com/package/qinojs) and [`@qino/qino` on JSR](https://jsr.io/@qino/qino).

## Quick start

Use [the Qino CMS starter](https://github.com/qinojs/qino/tree/main/module/starter.cms#getting-started) to create a working site in an empty project directory. The CMS runs from the main Qino repository. Start with the Bun setup in that guide.

Once the server is running, open [http://localhost:8080/](http://localhost:8080/) for the sample site or [http://localhost:8080/login](http://localhost:8080/login) for the editor sign-in. On the first run, the starter creates a local superuser. Follow the starter guide to sign in and switch on editing.

## Repository status

This repository is currently a placeholder. The CMS source still lives alongside the Qino core in the [qinojs/qino](https://github.com/qinojs/qino) repository.

## License

[MIT](LICENSE)
