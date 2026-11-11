# atom. — Chemistry Study Lab

An interactive chemistry learning website focused on the periodic table, main-group practice, molecular polarity, and a structured bonding/VSEPR syllabus.

**Built as a static website for GitHub Pages.** There is no server, database, API key, package manager, framework, or build step. The app can also be opened locally by opening `index.html` in a modern browser.

## Features

- **Interactive periodic table:** all 118 recognised elements, filter by metal / metalloid / nonmetal, search by name / symbol / atomic number, and inspect atomic number, abridged atomic mass, group, period, phase, classification, and valence-electron information.
- **Endless A-group quiz:** questions are drawn only from the s- and p-block main-group elements. Answer choices use the traditional IA–VIIIA labels. A wrong answer reveals the correct group and offers a direct link to the element's position in the table.
- **Molecular polarity quiz:** random molecule cards with polar / nonpolar choices. Every answer displays an explanation based on bond dipoles and molecular geometry.
- **Chemistry syllabus:** VSEPR notation and shape guide (including common AXₙEₘ patterns), ionic bonding, single/double/triple covalent bonds, coordinate covalent bonds, hydrogen-bond donor/acceptor criteria and non-examples, intermolecular forces, Van der Waals forces, and hybridisation.
- **Customisation:** light / dark / device theme, five accent colours, three text sizes, compact periodic-table mode, reduced motion, and four interface languages.
- **Saved progress:** quiz scores, streaks, and lesson completion are saved in the browser using `localStorage`.

## Languages

The interface supports **English, Bahasa Indonesia, Spanish, and French**. The extended syllabus articles and molecular-polarity explanations are available in **English and Bahasa Indonesia**. When Spanish or French is selected, the interface is translated while extended lesson and molecule explanations remain in English.

## Run locally

1. Extract the ZIP.
2. Open `index.html` in a recent browser.
3. No install command is needed.

The site uses only local HTML, CSS, and JavaScript assets. External links are provided only for optional reference reading.

## Publish on GitHub Pages

1. Create a GitHub repository (for example, `atom-chemistry-lab`).
2. Extract this ZIP and upload the **contents** of the `atom-study-lab` folder to the repository root. `index.html` must be at the root, not inside an extra nested folder.
3. Commit to the `main` branch.
4. Open **Settings → Pages** in the repository.
5. Under **Build and deployment**, choose **Deploy from a branch**.
6. Select branch `main` and folder `/ (root)`, then save.
7. Wait for GitHub Pages to publish the site. The published URL will appear in the Pages settings.

No custom build configuration is required.

## Project structure

```text
atom-study-lab/
├── index.html          # App layout and views
├── styles.css          # Responsive design, themes and colour systems
├── app.js              # Navigation, quiz logic, lessons, settings and persistence
├── data/
│   └── elements.js     # Compact 118-element reference dataset
├── assets/
│   └── favicon.svg     # Local app icon
├── README.md
├── DATA-CREDITS.md
└── LICENSE
```

## Chemistry and data notes

- The group quiz deliberately uses the traditional **A-group labels**: IA, IIA, IIIA, IVA, VA, VIA, VIIA, and VIIIA. These correspond to modern groups 1, 2, and 13–18.
- Hydrogen is located in group 1 for its one valence electron, but it is a nonmetal and is not an alkali metal. Helium is in group 18 but has two valence electrons.
- For transition and inner-transition elements, the idea of a single simple valence-electron count is not generally appropriate. The inspector therefore reports that the value is variable rather than pretending that the main-group shortcut applies.
- Atomic masses are abridged for readability. Square-bracketed entries indicate a representative isotope mass number for elements without a standard atomic weight. Values for the heaviest synthetic elements are not all measured.
- VSEPR is a qualitative shape-prediction model. The AX₃E₃ and AX₂E₄ rows are included as formal six-domain patterns; they are not presented as common stable neutral molecules.
- The `sp³d` / `sp³d²` hybridisation labels reflect a traditional introductory valence-bond model. Modern descriptions of hypervalent main-group bonding are more nuanced and often do not require substantial d-orbital participation.
- The listed intermolecular-force order is an introductory trend, not a universal ranking for all substances. Ionic/covalent bonding and intermolecular attractions are distinct categories.

## Sources for further study

- IUPAC, [Periodic Table of Elements](https://iupac.org/what-we-do/periodic-table-of-elements/) — element identities and standard atomic-weight reference.
- Staticdata.dev, [Periodic Table dataset](https://staticdata.dev/datasets/periodic-table/) — a structured 118-element reference, its field definitions, methodology, and upstream attribution.
- OpenStax, [Chemistry 2e](https://openstax.org/details/books/chemistry-2e) — open textbook background for atoms, bonding, molecular geometry, and intermolecular forces.
- Royal Society of Chemistry, [Periodic Table](https://www.rsc.org/periodic-table) — additional element reference material.

## Licence

The original application code is provided under the MIT License (see `LICENSE`). The element-reference data file is a compact educational dataset; see `DATA-CREDITS.md` for attribution and reuse notes.
