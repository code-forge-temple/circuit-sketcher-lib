# Contributing Image Assets

We welcome new circuit node images and exports, but to keep this project legally safe, please adhere to **all** of the following rules:

1. **You must be the original creator** of any image you upload **OR** the image must come from an open‐source project under a permissive license (e.g., CC0, MIT, Apache 2.0).

2. For each circuit node in your pull request, include a short declaration in a separate `ASSETS.md` file:
    - If you created both the image and the JSON yourself:
    > “I, `@your‐username`, created `my‐resistor.png` and `my‐resistor.json` and release them under CC0 1.0 Universal (https://creativecommons.org/publicdomain/zero/1.0/).”
     
    - If you have created the image with AI image generator:
    > “I, @your-username, created `my-symbol.svg` using ChatGPT (OpenAI) and release it under CC0 1.0 Universal (https://creativecommons.org/publicdomain/zero/1.0/).”
    
    - If it came from another project:
    > “`op‐amp.svg` is from [Example Repo](https://example.com), licensed under MIT (https://opensource.org/licenses/MIT).”

3. **Do not** upload images you do not own or that require non‐permissive (copyleft) or noncommercial licenses (e.g., CC BY‐NC, CC BY‐ND, GPL, AGPL).

4. Ensure filenames follow this convention: `component‐type.ext` (e.g., `ground‐symbol.svg`), all lowercase, with hyphens.

5. **Maintainers may remove or reject** any images whose provenance or license is unclear.

## Component Folder Structure

All contributed components must be placed in a new folder under the `assets` root directory.  
Each folder should be named after the component (all lowercase, hyphens for spaces), and must include:

- `my-component.svg` (preferred) or `my-component.png`: The image/icon for the component.
  It is recommended to use SVG format for best quality and scalability. You can use free tools like [Inkscape](https://inkscape.org) to create SVG images.
- `my-component.json`: The Circuit Sketcher "Export Node" JSON file for the component.  
  You can use either the Obsidian plugin or the [web version](https://code-forge-temple.github.io/circuit-sketcher-app/) of Circuit Sketcher to create this node, add your image, and define the ports (IO/Out/In ports), then export it.
- `ASSETS.md`: A declaration of authorship and license for the image and JSON.

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