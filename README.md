#[ juxt Theme](https://vscodethemes.com/e/Julius3722.juxt-theme/juxt-light)

Quiet themes for VS Code in the [juxt.ui](https://juliuss3722.github.io/juxt-library/) design language.

![alt text](https://i.imgur.com/E7qIoJJ.png)

The interface is grayscale, and the green `#079D6B` is kept for state: focus, the cursor, the active tab, selections, additions. Primary buttons use ink, not green. Code follows the juxt.ui docs highlighter: grayscale structure, green strings, amber constants, and types and components picked out in full contrast.

* **Juxt Dark**: `#09090b` background, zinc neutrals

* **Juxt Light**: `#fcfcfc` background, zinc neutrals

## Recommended settings

```jsonc
{
  "workbench.colorTheme": "Juxt Dark",
  "editor.fontFamily": "'JetBrains Mono', Consolas, monospace",
  "editor.fontSize": 13,
  "editor.lineHeight": 1.7,
  "window.autoDetectColorScheme": true,
  "workbench.preferredDarkColorTheme": "Juxt Dark",
  "workbench.preferredLightColorTheme": "Juxt Light"
}
```

## Development

The theme files in `themes/` are generated from the tokens in `build.mjs`, which mirror `packages/ui/src/styles/tokens.css` and the docs' Shiki themes.

```bash
npm run build     # regenerate themes/*.json
npm run package   # build a .vsix
```

Press <kbd>F5</kbd> in this folder to try the themes in an Extension Development Host.
