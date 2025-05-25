# Circuit Sketcher Component Library

This repository provides a curated library of circuit component images and icons for use with [circuit-sketcher-obsidian-plugin](https://github.com/code-forge-temple/circuit-sketcher-obsidian-plugin) and [circuit-sketcher-app](https://github.com/code-forge-temple/circuit-sketcher-app).

## Project Purpose

The goal of this project is to offer a collection of open, permissively licensed circuit element node images/exports that can be easily integrated into the Circuit Sketcher ecosystem ([circuit-sketcher-obsidian-plugin](https://github.com/code-forge-temple/circuit-sketcher-obsidian-plugin) and [circuit-sketcher-app](https://github.com/code-forge-temple/circuit-sketcher-app)).

## How to Use

- **For Users:**  
  Download or clone this repository and use the images in your own projects, or reference them directly in the supported plugins/apps.
- **For Developers:**  
  Integrate these assets into your plugin or app by following the usage instructions in your tool’s documentation.

## Directory Structure

All contributed components are organized under the `assets` root folder.  
Each user should create a pull request with a new folder named after the component they want to add (e.g., `my-component`).  
Inside each component folder:

- `my-component.svg` (preferred) or `my-component.png`: The image/icon for the component.
  It is recommended to use SVG format for best quality and scalability. You can use free tools like [Inkscape](https://inkscape.org) to create SVG images.
- `my-component.json`: The Circuit Sketcher `Export Node` JSON file for the component.  
  You can use either the Obsidian plugin or the [web version](https://code-forge-temple.github.io/circuit-sketcher-app/) of Circuit Sketcher to create this node, add your image, and define the ports (IO/Out/In ports), then export it.
- `ASSETS.md`: A declaration of authorship and license for the image and JSON.

**Naming convention:**  
The folder name, image file, and JSON file must all use the same name (all lowercase, hyphens for spaces).

**Example:**
```
assets/
  resistor/
    resistor.svg
    resistor.json
    ASSETS.md
  op-amp/
    op-amp.svg
    op-amp.json
    ASSETS.md
```

## Image Asset Policy 🚨

**`circuit-sketcher-lib`** contains only user‐submitted images (circuit element icons, node pictures, etc.). To avoid copyright issues, **we do not accept** any images unless:

- They were **created by the contributor themself** (and are released under CC0, MIT, or other OSI‐approved permissive licenses),  
- OR they come from an **external open source project** with a clearly stated permissive license (e.g., “This icon is from [Project X] under MIT: https://opensource.org/licenses/MIT”).  

By using these assets, you agree that they are properly licensed. If you need to add or modify an image, please follow the contribution steps in [CONTRIBUTING.md](./CONTRIBUTING.md).

## How to Contribute

We welcome new circuit element icons and node images! Please read [CONTRIBUTING.md](./CONTRIBUTING.md) for detailed guidelines on submitting assets, licensing requirements, and naming conventions.

---

**Questions or suggestions?**  
Open an issue or start a discussion!

## License

All original assets in this repository are released under [CC0 1.0 Universal (Public Domain Dedication)](https://creativecommons.org/publicdomain/zero/1.0/), unless otherwise noted in the component's `ASSETS.md`.