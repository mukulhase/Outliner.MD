> **Unofficial fork.** This is a patched build of
> [Quorafind/Outliner.MD](https://github.com/Quorafind/Outliner.MD) maintained
> only so the fix in
> [Quorafind/Outliner.MD#107](https://github.com/Quorafind/Outliner.MD/pull/107)
> can be installed via BRAT while that PR is open: the frontmatter regex in
> `OutlinerEditorView.setState` was greedy, so any note containing a `---`
> thematic break rendered only the part after the *last* `---`.
>
> Releases here are versioned `0.1.14+` to sort above upstream's `0.1.13`. If
> upstream releases again, retire this fork and go back to the upstream repo.
> All credit and copyright remain with the original author; distributed under
> the upstream FSL-1.1-Apache-2.0 licence.

# Obsidian Outliner View

<div align="center">

![GitHub Release](https://img.shields.io/github/v/release/quorafind/outliner.md) ![GitHub Downloads](https://img.shields.io/github/downloads/quorafind/outliner.md/total)

</div>

A powerful outliner (editor) view plugin for Obsidian that makes your notes work like Workflowy, Dynalist, and Roam Research.

## Features

### 💭 Smoother Outliner Experience

Filter, hotkey, and more - just like you are using professional outliner software.

### 💫 Embedded Content Editing

Embed anything and edit it directly in place.

### 📚 Backlink Editing

Open your note, scroll to the bottom, and edit backlinks directly without switching contexts.

### 📝 Note as Notebook

Use notes as notebooks and manage sections efficiently.

## Installation

### From GitHub Releases

1. Download the latest release from [GitHub Releases](https://github.com/quorafind/outliner.md/releases)
2. Extract main.js, manifest.json, and styles.css to your vault's .obsidian/plugins/outliner-md/ folder
3. Reload Obsidian
4. Enable the plugin in Settings → Community Plugins

### From Source

```bash
git clone https://github.com/quorafind/outliner.md.git
cd outliner.md
pnpm install
pnpm run build
```

## Development

```bash
pnpm install
pnpm run dev      # Development mode with hot reload
pnpm run build    # Production build
pnpm run lint     # Lint code
```

## Usage

> [!warning]
> You need to add \`outliner: true\` to the frontmatter of your note to enable the outliner view.

### Recommended Plugins

- **Obsidian Zoom** - Enhanced focus mode
- **Obsidian Outliner** - Additional outliner features
- **Obsidian Dataview** - Query and display your data

## License

This project is licensed under the **Functional Source License, Version 1.1, Apache 2.0 Future License** (FSL-1.1-Apache-2.0).

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

---

Made with ❤️ for the Obsidian community
