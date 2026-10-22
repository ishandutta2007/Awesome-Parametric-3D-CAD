# Awesome-Parametric-3D-CAD

# Top Parametric 3D CAD Tools Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Feature-History Modeling, B-Rep Kernels & Browser-Native Design*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Parametric 3D CAD**. These tools let engineers and designers build solid models through feature histories — sketches, extrudes, fillets, and assemblies — where changing a dimension updates the entire model rather than breaking it.

**Examples** include FreeCAD, CycleCAD, CadQuery, OpenSCAD, SolveSpace, SolidWorks, Fusion 360, Onshape, Siemens NX, and PTC Creo (the category leaders).

**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, B-Rep solid modeling, and code-driven design — ideal for mechanical engineers, hardware startups, and makers who need professional-grade parametric modeling without $4,000–$8,000 per-seat licenses.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Onshape](https://www.onshape.com/)**  
  **Browser-based parametric CAD created by former SolidWorks developers** — the workflow is intentionally similar, making it the easiest free transition for SolidWorks users . **Free tier available** but **all models are public** on the free plan . **No installation required** — runs on any laptop or Chromebook . **Best for beginners and teams wanting SolidWorks-like parametric modeling without installs**, accepting the public-model trade-off on the free tier [citation:1][citation:6].

- **[Fusion 360](https://www.autodesk.com/products/fusion-360/)**  
  **Autodesk's integrated CAD/CAM/CAE platform** — free for personal, non-commercial use with up to **10 active editable documents**. **The closest free workflow to SolidWorks** for learners: sketch → extrude → pattern feels nearly identical . **Includes CAM toolpaths** that FreeCAD lacks, making it the pragmatic hybrid choice for manufacturing . **Best for hobbyists and startups** wanting parametric CAD plus CAM, accepting cloud dependency and commercial restrictions [citation:1][citation:3][citation:6].

- **[SolidWorks](https://www.solidworks.com/)**  
  **The industry standard for mechanical design** — feature-based parametric modeling with the deepest assembly and drawing toolchain. **Costs roughly $4,000–$8,000 per seat** and requires Windows . **Best for professional engineering teams** where supplier and customer workflows demand native SolidWorks files [citation:1].

- **[Siemens NX](https://plm.sw.siemens.com/en-US/nx/)**  
  **Enterprise-grade CAD/CAM/CAE** for complex products and large assemblies. High licensing cost, steep learning curve, and deep integration with Siemens PLM.

- **[PTC Creo](https://www.ptc.com/en/products/creo)**  
  **Parametric CAD for discrete manufacturers** with strong surfacing, simulation, and PLM integration. Enterprise pricing.

## Open-Source GitHub Projects

- **[FreeCAD](https://github.com/FreeCAD/FreeCAD)**  
  **The leading open-source parametric 3D CAD modeler** — LGPL-2.1 licensed, **34,000+ GitHub stars**, actively developed with weekly builds [citation:2][citation:12]. **Feature-based parametric modeling with full history** through the Part Design workbench, constraint-based Sketcher, and modular workbenches for FEM, CAM/Path, Arch/BIM, and TechDraw drafting . **Python scripting** for automation and custom tools, plus an active addon ecosystem . **100% free with no commercial restrictions, no tracking, and no cloud dependency** . **Trade-offs**: **UI is rougher than commercial tools** and the learning curve is steeper ; **complex assemblies slow down** — performance drops noticeably beyond 100+ parts ; **CAM is weak** compared to Fusion 360 ; **occasional stability issues** and **no professional support** make it risky for production-ready OEM workflows [citation:3][citation:6][citation:11]. **Best for mechanical engineers, product designers, and makers** needing advanced parametric modeling and simulation without paying for SolidWorks or Fusion 360 [citation:11].

- **[CycleCAD](https://github.com/vvlars-cmd/cyclecad)**  
  **The browser-native parametric CAD with a real B-Rep kernel** — MIT licensed, runs entirely in the browser using **OpenCascade.js (WASM)** — the same geometry engine behind FreeCAD and KiCad . **Real solid modeling with true fillets and booleans**, no install and no login . **Text-to-CAD** converts natural language to 3D geometry with live preview; **Photo-to-CAD** turns a phone photo into a parametric model . **DFM feedback** for 9 processes and 20+ materials; **generative design** with SIMP topology optimization; **multi-physics simulation** (FEA, thermal, modal, drop test) in-browser . **Agent API** with 55 commands across JSON-RPC, MCP server, CLI, and REST . **STEP import/export** with a full 2D drawing workspace . **Best for users wanting real B-Rep CAD without installing anything** — the browser-native alternative to Onshape with no cost or public-model requirement [citation:4].

- **[CadQuery](https://github.com/CadQuery/cadquery)**  
  **The Python parametric CAD scripting framework** — Apache-2.0 licensed, **5,900+ GitHub stars** [citation:12]. **Design parts by writing Python code, not clicking** — fully parametric by nature, Git-compatible (design files are code), and repeatable (same code → same geometry every time) . **Pairs with the Python ecosystem** (NumPy, Pandas) for engineering automation . **Built on OpenCASCADE** with STEP export, lofting between dissimilar surfaces, and spline support . **Trade-offs**: **steep learning curve** — you must code; **assembly support is awkward**; **3D preview is basic**; **no manufacturing drawings or GD&T** [citation:3]. **Best for generating parametric design families** — 50 bracket variants by changing code parameters — and DevOps-style CAD version control [citation:3][citation:7].

- **[OpenSCAD](https://github.com/openscad/openscad)**  
  **The programmer's solid 3D CAD modeler** — **10,000+ GitHub stars** [citation:12]. **Script-based CSG modeling** where you describe geometry in code and OpenSCAD renders it . **Fully parametric** — change a variable and regenerate the model; **version-control friendly** with plain-text source files . **Exports STL for 3D printing** . **Trade-offs**: **no visual interactive modeling** — organic or sculpted shapes are impractical; **requires learning the scripting language** . **Best for programmers and 3D printing enthusiasts** who value precision and reproducibility over visual editing [citation:11].

- **[SolveSpace](https://github.com/solvespace/solvespace)**  
  **The lightweight, clean parametric CAD for Linux and beyond** — GPL-3.0 licensed, **4,200+ GitHub stars** [citation:12]. **Reduces itself to a very simple interface** without the clutter and feature overload that makes FreeCAD suffer . **The underlying solving engine makes sense and the interface is clean**, enabling a fast workflow . **Cross-platform compatible** . **Trade-offs**: **lacks features** like chamfer and fillet tools as base examples; parameters and variables are missing on the main branch (available on a branch) . **Best for users wanting a fast, focused parametric sketcher** without FreeCAD's complexity [citation:15].

- **[LibreCAD](https://github.com/LibreCAD/LibreCAD)**  
  **The mature 2D drafting tool** — GPL-2.0 licensed . **Handles complex 2D geometry as well as commercial tools** with DWG/DXF support, layers, blocks, and hatching . **Runs on older hardware** without performance issues . **Trade-offs**: **2D only** — no 3D modeling or assembly; **no parametric constraints** — dimensions are fixed values . **Best for architectural floor plans, electrical schematics, and 2D manufacturing drawings** where 3D CAD is overkill [citation:3][citation:11].

### Additional Strong Open-Source Options

- **SolidCraft** — AI-assisted Rust parametric 3D CAD with MCP server for agent-driven modeling. Early but usable for simple parts; 75 of 76 reference parts match FreeCAD-computed volumes . Apache-2.0 licensed, ~2.9k stars [citation:9].
- **build123d** — Python parametric CAD library, Apache-2.0 licensed, 3,400+ stars. Code-first alternative to CadQuery with a more Pythonic API [citation:12].
- **Blender + CAD Sketcher** — Blender is mesh-based, but the CAD Sketcher addon adds constraint-based parametric workflows for precision modeling alongside organic sculpting [citation:6][citation:11].
- **jsketcher** — Parametric 2D and 3D modeler in pure JavaScript. 1,700+ stars, browser-based [citation:8].

**Frameworks for building custom systems**: Combine **FreeCAD** for full parametric modeling with FEM and CAM workbenches in a desktop environment, **CycleCAD** for browser-native B-Rep modeling with text-to-CAD and in-browser simulation, **CadQuery** for code-driven design families and DevOps-style version control, **OpenSCAD** for script-based CSG and 3D printing, and **SolveSpace** for a clean, focused parametric sketcher — to build a CAD stack tailored to your platform (desktop vs browser), workflow (visual vs code), and manufacturing needs.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Parametric 3D CAD tools differ significantly in modeling paradigm, kernel reliability, and assembly performance. **FreeCAD is the most capable open-source desktop option** but its **complex assembly performance drops beyond 100+ parts**, CAM is weak, and it lacks professional support — risky for production-ready OEM workflows [citation:3][citation:11]. **CycleCAD runs real B-Rep solid modeling in the browser** via OpenCascade.js WASM, with no install and no public-model requirement — a different trade-off than Onshape's free tier [citation:4][citation:6]. **CadQuery and OpenSCAD require coding** — powerful for automation and repeatable design families, impractical for visual iterative design [citation:3][citation:11]. **SolveSpace's solver is clean and fast** but lacks fillet/chamfer tools and parameter support on the main branch [citation:15]. **Commercial tools like SolidWorks remain the career standard** — skills learned in FreeCAD, Fusion 360, or Onshape transfer, but supplier workflows may still require native files [citation:1].
- Self-hosted open-source solutions require proper GPU drivers for 3D viewport performance, sufficient RAM for complex models (16 GB recommended for FreeCAD and Blender), and backup of project files in neutral formats like STEP for portability.

---

**Made for mechanical engineers, product designers, hardware startups, and makers building parametric 3D models.**
Let's make parametric 3D CAD more open, accessible, and browser-native.
