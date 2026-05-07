# AI Web Agent

Open-source AI web automation Chrome extension with a multi-agent system and support for multiple LLM providers.

## Build from source

1. **Prerequisites**: [Node.js](https://nodejs.org/) v22.12.0 or higher, [pnpm](https://pnpm.io/installation) v9.15.1 or higher (see `.nvmrc` and root `package.json` engines).

2. **Install dependencies** (from the repository root):

   ```bash
   pnpm install
   ```

3. **Build** the extension:

   ```bash
   pnpm build
   ```

   Output is written to the `dist/` directory.

4. **Optional**: create a zip for distribution:

   ```bash
   pnpm zip
   ```

   Output goes to `dist-zip/`.

5. **Load in Chrome**: open `chrome://extensions/`, enable **Developer mode**, click **Load unpacked**, and select the `dist/` folder.

6. **Optional — development**: run `pnpm dev` for watch builds; reload the extension on `chrome://extensions/` after changes.

### Icons

This fork ships without toolbar/store icons. Add `icon-32.png` and `icon-128.png` under `chrome-extension/public/`, then restore `action.default_icon`, top-level `icons`, and the icon entries in `web_accessible_resources` in [`chrome-extension/manifest.js`](chrome-extension/manifest.js).

## License

Apache License 2.0 — see [LICENSE](LICENSE).
