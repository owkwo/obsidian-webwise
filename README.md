# obsidian-webwise

obsidian-webwise is an experimental Obsidian plugin for importing Supernotes cards into an Obsidian vault. It downloads cards through the Supernotes API, converts card metadata to flat frontmatter properties, writes note content, and can optionally change the remote card state after import.

## Technical stack

- TypeScript
- Obsidian plugin API
- esbuild
- Luxon, i18next, and Popper
- Supernotes HTTP API

## Development

```sh
npm install
npm run build
npm run dev
```

Manual testing requires an Obsidian vault and a Supernotes API key. Never commit API keys or a real vault.

## Status

Work in progress. One-way download/import is implemented; robust synchronization is not.

## Known limitations

- The package and plugin manifest still use the historical “obsidian-supernotes” identifier; changing it requires a migration plan for existing installations.
- Synchronization is primarily Supernotes-to-Obsidian and conflict handling is incomplete.
- Remote deletion/disable operations are destructive and need stronger safeguards.
- API behavior is not covered by contract tests.
- Some dependencies and build configuration are from an older Obsidian template.

## Next steps

Define identity and conflict rules, add dry-run and backup behavior, test API failures and rate limits, modernize the build stack, remove undocumented API assumptions, and publish signed/versioned releases.
