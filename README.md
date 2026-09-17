# Vector Design Utilities Prototype ver.

A browser-based SVG/vector utility suite for grid generation, placeholder composition, pattern construction, metadata authoring, and SVG optimization/inspection.

> Packaging note: `#Grid-generator-reFIX.html` is copied byte-for-byte to `index.html`. No application code or UI is modified.

## Main Workspaces

The source contains four primary tabs:

1. **Grid Generator**
2. **Placeholder Gen**
3. **Pattern Constructor**
4. **SVG Optimizer & Inspector**

## 1. Grid Generator

Grid Generator provides several editable grid systems, including:

- Bento Grid
- Normal Grid
- Grid Lines

The workspace supports configurable canvas dimensions, aspect-ratio locking, grid settings, colors, radii, and related layout controls.

Generated vector output can be exported as:

- SVG
- EPS

Export options include SVG version and text encoding choices.

## 2. Placeholder Gen

Placeholder Gen creates vector placeholder compositions with:

- width / height controls,
- common aspect-ratio presets,
- background and text colors,
- custom text,
- system/local font workflow,
- pan and zoom preview,
- editable metadata.

Output formats include:

- SVG
- EPS
- JPG
- WebP

## 3. Pattern Constructor

Pattern Constructor creates repeated vector/raster pattern compositions.

Built-in motif types include:

- Dots
- Cross
- Grid Box
- Diagonal Strip
- Custom SVG

Controls include:

- canvas size,
- aspect presets,
- motif count,
- spacing/layout,
- foreground/background colors,
- transparency,
- text overlay,
- imported custom SVG,
- pan/zoom preview.

The source supports canvas dimensions up to 2160 px per side in the relevant controls.

Exports include:

- SVG
- EPS
- JPG
- WebP

Pattern export can also carry editable/basic metadata.

## 4. SVG Optimizer & Inspector

Accepts SVG files only and provides a safer optimization/inspection workflow.

Features include:

- before/after SVG previews,
- pan/zoom,
- source/output size comparison,
- SVG code output,
- copy optimized SVG code,
- structure/geometry inspection,
- editable portable metadata,
- metadata locking in the app,
- SVG and EPS export.

Optimization controls include options for:

- comments,
- editor metadata,
- empty nodes,
- unused IDs,
- default attributes,
- minification,
- path simplification,
- overlap handling,
- extrema,
- path direction normalization,
- inflection handling,
- numeric precision.

## Portable SVG Metadata

The source can embed standards-oriented metadata using namespaces such as:

- RDF
- Dublin Core
- Creative Commons

Metadata fields include items such as:

- file name/title,
- file size,
- created/modified dates,
- authors,
- tags,
- description,
- copyright,
- comments.

Metadata can be locked and saved in the browser for the imported SVG.

## SVG Export Settings

Relevant vector workspaces support options such as:

- SVG 1.0 / 1.1
- UTF-8 / UTF-16
- merged/union or separate vector behavior where exposed

Pattern and optimizer workflows also provide EPS output.

## Session Autosave

The app contains refresh-safe session persistence.

It uses:

- `localStorage` for interface/session state,
- IndexedDB for cached SVG Optimizer source data.

A Refresh Session action clears stored working state and reloads the app.

## External Dependency

### Tailwind CSS CDN

```text
https://cdn.tailwindcss.com
```

Purpose: application styling.

No other runtime JavaScript CDN is required by the supplied source.

## External Creator Link

```text
https://www.instagram.com/efcreative.dsg
```

Other HTTP URLs found in the source primarily identify SVG/XML/RDF namespaces.

## Browser APIs

Important APIs include:

- SVG DOM
- DOMParser / XMLSerializer
- Canvas 2D
- File API
- Blob / Object URLs
- Clipboard API
- localStorage
- IndexedDB
- native image encoding
- browser downloads
- local/system font access where supported

## Running Locally

Open:

```text
index.html
```

or serve it with:

```bash
python -m http.server 8080
```

The unchanged source requires internet access for Tailwind CDN styling on a fresh load.

## GitHub Pages

This is a static frontend and can be deployed through GitHub Pages.

## Project Structure

```text
.
├── index.html
├── README.md
└── .gitignore
```

## Copyright

The supplied source states:

```text
©2026 Ervin Faristiyanto. All rights reserved.
```

No project-wide `LICENSE` is added by this packaging step.
