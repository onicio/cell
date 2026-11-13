# Cell Explorer 3D

Cell Explorer 3D is an interactive website about the cell, made for grade 9 biology (Unit 2). Students turn a 3D cell with the mouse or a finger, click or tap on each organelle to learn what it does, read short lessons and answer a quiz.

The whole site is one file, `cell-explorer.html`. It needs no installation, no build step and no server code. The 3D library and the fonts are inside the file, so the page loads nothing from other servers and also works offline.

## What is in the site

### Explore in 3D

- Three models: an animal cell, a plant cell and a bacterium.
- Drag to turn the cell, scroll or pinch to zoom, click or tap a part to open its card.
- To move the view, hold `Shift` and drag, or drag with the right mouse button. On a touch screen, drag with two fingers. The **Reset view** button brings back the whole cell.
- A cell with a wall has more than one boundary layer. Click the edge of the cell again to go to the next layer: in the plant cell from the cell wall to the plasma membrane, in the bacterium from the capsule to the cell wall and then to the plasma membrane.
- The small and thin parts, such as the ribosomes, the vesicles, the cytoskeleton and the pili, have a click area that is bigger than their drawing. This makes them easier to hit with a finger.
- Each card gives the name and how to say it, the membrane type, the job of the part, a short explanation, an everyday comparison, a few key facts and where to find the part in the model.
- A filter sorts the parts by membrane: double membrane, single membrane or no membrane.
- **Follow a protein** is a tour in 7 steps, from the DNA in the nucleus to exocytosis at the plasma membrane.
- **Find it** is a game. It shows a clue and the student clicks the right part, in the model or in the parts list. A round has up to 8 clues, with two tries for each clue. Only an answer on the first try scores a point. For a very small part, such as the ribosomes, a near miss counts. For a boundary layer, such as the plasma membrane, a click on the edge of the cell counts.
- Three buttons turn on and off the slow spin, the labels and the focus mode. With the focus mode on, the other parts fade when one part is selected.
- A scale bar shows the real size, in µm or nm, and changes with the zoom.

The models have 22 parts:

| Group | Parts |
| --- | --- |
| Double membrane | nucleus, mitochondria, chloroplasts |
| Single membrane | rough ER, smooth ER, Golgi apparatus, vesicles, lysosomes, vacuoles, central vacuole |
| No membrane | ribosomes, nucleolus, centrioles, cytoskeleton. In the bacterium also the nucleoid, plasmids, flagellum and pili |
| Boundary and filling | plasma membrane, cytoplasm, cell wall, capsule |

### Lessons

Eight short chapters, with figures that the student can change:

| Chapter | Content |
| --- | --- |
| 1. Cell theory | the three principles, Hooke and Leeuwenhoek |
| 2. Two kinds of cells | prokaryotes and eukaryotes, plant and animal cells, a comparison table |
| 3. Organelles | organelles with and without a membrane, the job of each part, a size ruler |
| 4. Plasma membrane | the phospholipid, the lipid bilayer, membrane proteins, selective permeability |
| 5. Transport | diffusion, facilitated diffusion, osmosis, active transport, hypotonic, isotonic and hypertonic solutions, endocytosis and exocytosis |
| 6. Cell size | the surface area to volume ratio, with a box that changes with three sliders |
| 7. Cell cycle and mitosis | interphase, the stages of mitosis, cytokinesis in animal and plant cells, G0, binary fission |
| 8. Cancer | benign and malignant tumors, drugs that block mitosis |

### Quiz

The quiz uses the questions of the class study guide for Unit 2.

- **Part A** has 16 matching items. The page checks them.
- **Part B** has 34 questions. The page checks questions 31 to 34. For questions 1 to 30 the student writes an answer, opens the model answer and then marks the question with **I had it** or **Review again**.
- A progress bar counts 35 items: Part A and the 34 questions.
- The answers are saved in the browser, so they are still there when the page is opened again. They stay on that device only. The **Start over** button erases them.

Two notes about the answers:

- The model answers were written for this site. They are not an official answer key, so compare them with the class notes.
- Question 34 asks for the surface area to volume ratio of three boxes. The page accepts the real surface area, which is 38 cm² for the 3 × 4 × 1 box. The shortcut printed on the study guide (length × width × number of sides) is right only for a cube, and it gives 72 cm² for that box. The model answer explains the difference.

## Put it online with GitHub Pages

1. Create a repository on GitHub, or open one that you already have. With a free GitHub account the repository must be public.
2. Upload `cell-explorer.html` to the repository.
3. Open **Settings**, then **Pages**.
4. Under **Build and deployment**, set **Source** to **Deploy from a branch**. Select your main branch and the folder `/ (root)`, then click **Save**.
5. Wait a few minutes. The page is then at `https://<username>.github.io/<repository>/cell-explorer.html`.

For a shorter address, rename the file to `index.html`. The page then opens at `https://<username>.github.io/<repository>/`. Do this only in a repository or folder that has no `index.html` yet. If there is one, the upload replaces it.

To update the site later, upload the new version of the file with the same name.

GitHub describes these settings in [Configuring a publishing source for your GitHub Pages site](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site).

## Direct links

Add `#lessons` or `#quiz` to the address to open that section directly. For example, an address that ends in `cell-explorer.html#quiz` opens the quiz.

## Use it without the internet

Download `cell-explorer.html` and open it with a double click. The page works from the disk, and the quiz answers are still saved.

## On a phone or tablet

On a small screen the 3D view fills the whole screen, and the panels fold away to leave room for the cell.

- A short bar at the bottom shows the name of the selected part. Tap the bar, or swipe it up, to open the panel with the details and the parts list. Tap **Close**, or swipe the top of the panel down, to fold it again.
- A part chosen from the parts list folds the panel, so the part can be seen in the model.
- When the phone is held sideways, the cell is on the left and the panel is on the right.
- One finger turns the cell, a pinch zooms, two fingers move the view and a tap selects a part.
- The **Whole cell** button goes back from a selected part to the whole cell. After a zoom or a move, the same button is named **Reset view**.
- The labels start turned off. When they are on, a drag or a pinch can also start on a label.
- The width of the window decides the layout, not the kind of device. A computer window that is narrower than 1080 px gets the same layout.

## Browsers and devices

- The 3D view needs a browser with WebGL. Current versions of Chrome, Edge, Firefox and Safari have it.
- The page was tested in Chrome, at computer, tablet and phone screen sizes: every part of the three cells, the tour, the game, the lesson figures, the quiz checks and the saving of answers. The touch gestures were tested with the touch input that Chrome can simulate. The page was not tested on a real phone or tablet yet, and not in other browsers.
- If WebGL is not available, a message takes the place of the 3D view. The parts list, the cards, the tour, the lessons and the quiz still work.
- On a screen with many pixels the 3D view is drawn at up to twice the normal resolution. If the device then draws it slowly, under about 22 pictures per second, the page lowers the resolution in steps. The picture gets a little softer and the movement gets smoother.
- The page follows the light or dark setting of the device.
- If the device is set to reduce motion, the slow spin is off and the camera moves without animation.
- Keyboard: when the 3D view has the focus, the arrow keys turn the cell, `+` and `-` zoom, and `Esc` goes back to the whole cell.

## Privacy

The page has no tracking, no cookies and no accounts, and it sends no data to any server. The quiz answers are kept in the local storage of the browser, under the key `cellx-quiz`.

## Change the content

All the content is in `cell-explorer.html`. Open the file in a code editor and search for these names:

| Search for | What it holds |
| --- | --- |
| `const ORG` | every part of the cell: name, pronunciation, membrane type, job, text, comparison, facts and the clue for the game |
| `const CELLS` | the three cell types and the parts that each one has |
| `const TOUR` | the steps of the protein tour |
| `const MATCH` | the terms and descriptions of quiz Part A |
| `const QB` | the questions and model answers of quiz Part B |
| `id="pageLessons"` | the text of the lessons, in plain HTML |
| `--bg-a` | the start of the colors and fonts, as CSS variables. The light values come first, then the dark values |

When you edit a text, keep the quotes, commas and brackets around it as they are.

The file also has two long blocks that should stay as they are:

- the fonts, four very long lines near the top, after the comment `Embedded fonts`
- the three.js library, after the comment `Embedded library`

The code of the page itself starts after the comment `Page code`.

The fonts inside the file cover the Latin alphabet, which is enough for English, Spanish, Portuguese, French and similar languages. Any other character is shown with a font of the device.

## Notes on the models

- The models are simplified and not to scale. Ribosomes and vesicles are drawn bigger than they are, so that they can be seen.
- The nucleus, the mitochondria, the chloroplasts and the bacterium have a piece cut away to show the inside.
- The sizes on the cards are typical values and they are approximate.
- The cell cycle wheel in chapter 7 is drawn for a human cell that divides once every 24 hours: G1 11 hours, S 8 hours, G2 4 hours, M 1 hour.

## Files

| File | What it is |
| --- | --- |
| `cell-explorer.html` | the site, a little under 1 MB. Most of it is the 3D library (about 600 KB) and the fonts (about 195 KB) |
| `README.md` | this file |

## Credits

The file includes this open source work:

| Component | License | Copyright |
| --- | --- | --- |
| [three.js](https://threejs.org) r128 | MIT | Copyright © 2010-2021 three.js authors |
| [Bricolage Grotesque](https://github.com/ateliertriay/bricolage) | SIL Open Font License 1.1 | Copyright 2022 The Bricolage Grotesque Project Authors |
| [Lexend](https://github.com/googlefonts/lexend) | SIL Open Font License 1.1 | Copyright 2019 The Lexend Project Authors |
| [IBM Plex Mono](https://github.com/IBM/plex) | SIL Open Font License 1.1 | Copyright 2017 IBM Corp. |
