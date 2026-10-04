# Persona 3 Reload Companion

A static fan-made reference for **Persona 3 Reload** and **Episode Aigis**, adapted from the supplied Persona 4 Golden Companion. No framework or hosted API is needed to run it.

## Guide contents

- **Interface:** Restored Daily Field Guide, first-edition hero headline and chapter headings; a tilted midnight clock replaces the decorative 03. The guide panels animate open and closed, with reduced-motion support.
- **Social Links:** All 22 Arcana with availability, unlock conditions, 390 ordered rank-dialogue answer entries, relationship choices, individual name-spoiler toggles and 220 rank checkboxes. The ★ notation identifies affinity values when provided. Choices are in dialogue order; a slash separates equally useful alternatives or relationship branches. Some mandatory story scenes have no point-affecting choices.
- **Classroom:** 52 classroom and exam answers arranged by month.
- **Elizabeth:** All 101 base-game requests, with conditions, deadlines, rewards, solutions and progress tracking.
- **Linked Episodes:** 25 trackable linked-episode dates.
- **Tartarus:** All 11 block segments, guardian-floor checklist and an expanded searchable main-game bestiary with **292 Shadow, guardian, Monad and finale entries** across Thebel–Adamah. A question mark means an affinity *has not been independently verified*; "None" means a confirmed absence of a weakness. A reference link is included for further affinity details.
- **Fusion:** Link to an external Persona 3 Reload-specific fusion calculator.
- **Episode Aigis:** An independent bottom-of-page DLC section with the eight Abyss of Time doors, floor ranges, guardian checkpoint guidance, 25 trackable checkpoints, all 59 DLC Elizabeth requests with solutions and rewards, and door-specific walkthrough links. Both DLC trackers save separately from the main game. The DLC enemy affinity bestiary is available through the linked guide.

## Running locally

Extract the ZIP and open `index.html`. Alternatively, open the provided `Persona-3-Reload-Companion-v3.htm`, which embeds the HTML, CSS, JavaScript and game data in one file. Local progress is saved when browser local storage is available. Standalone-file progress and published-site progress are separate browser origins; use the gear icon to export and import saves.

## Deploying on GitHub Pages

1. Make a GitHub repository (e.g. `P3R-Companion`).
2. Upload the contents of this ZIP to the repository root, preserving the `icons/` directory.
3. Open **Settings → Pages**, select **Deploy from a branch**, and select `main` / `/ (root)`.
4. Wait for the deployment, then open `https://YOUR-USERNAME.github.io/P3R-Companion/`.
5. Reload once online after updating files. The new service worker cache name is `p3r-companion-v3`.

The website makes no font, image or JS requests to third parties. External walkthrough and fusion links naturally require a connection.

## Editable data and rebuilding

Editable sources are `build.py`, `social_answers.txt`, `enemies_extra.txt`, `aigis_requests.txt` and `enhance.py`. Run `python enhance.py` to regenerate the enhanced `social.json`, `tartarus.json`, `aigis.json` and `data.js`. Run `python patch_app.py` **only on the original HTML/JS/CSS files**, because it appends the new styles; it is supplied for reference rather than for repeated rebuilds. The `patch_v3.py` script is a one-time visual update and must not be rerun on already-patched sources. Run `python package.py` to package the existing V3 sources. Update the service-worker cache name after changing deployed assets.

## References

- [Reload Social Link dialogue](https://www.inverse.com/gaming/persona-3-reload-social-links-guide-all-answers), [GameFAQs Social Link guide](https://gamefaqs.gamespot.com/pc/409941-persona-3-reload/faqs/81170/social-links)
- [Classroom / exams](https://www.powerpyx.com/persona-3-reload-all-class-and-exam-question-answers/)
- [Elizabeth requests](https://www.powerpyx.com/persona-3-reload-elizabeth-request-guide/)
- [Linked Episode dates](https://www.escapistmagazine.com/persona-3-reload-linked-episodes-rewards-dates/)
- [Main-game Shadow list](https://megatenwiki.com/wiki/Shadows_in_Persona_3_Reload), [affinity guide](https://steamcommunity.com/sharedfiles/filedetails?id=3415170366)
- [Episode Aigis door guide](https://game8.co/games/Persona-3-Reload/archives/471612), [Abyss walkthrough](https://game8.co/games/Persona-3-Reload/archives/472757), [DLC requests](https://primagames.com/gaming/how-to-complete-all-episode-aigis-elizabeth-requests-in-persona-3-reload)
- [Fusion calculator](https://aqiu384.github.io/megaten-fusion-tool/p3r/personas)

Persona 3 Reload and all related names belong to ATLUS / SEGA. This is an independent, unofficial fan project.