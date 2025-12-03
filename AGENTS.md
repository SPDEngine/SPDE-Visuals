# Repository Guidelines

## Project Structure & Asset Organization
- Root: overview in `README.md`, this `AGENTS.md`, and a sample talk `Talk-LeChen-AMS_GeorgiaTech.pdf`.
- `Peak-propogation/`: simulation data (`.dat`) and derived plots (`.eps`, `.pdf`, `.jpeg`) for stochastic heat equation peak propagation.
- `Some_images_by_AI/`: AI-generated images (`.png`) intended for slides, posters, and illustrations.
- Add new subdirectories only when they group a clear theme (e.g., a new SPDE model or talk).

## Build, Preview, and Development Workflow
- This repository contains static assets only; there is no build system or automated tests.
- Preview figures directly with your viewer, e.g. `xdg-open Peak-propogation/small_Delta_L4_cut.pdf` or `xdg-open Some_images_by_AI/MJ_SHE.png`.
- When adding plots generated from code, add a short note to the nearest `README.md` explaining how they were produced (tool, script, and main parameters).

## File Naming & Styling Conventions
- Use descriptive, ASCII-only filenames without spaces; follow existing patterns such as `small_Delta_Lk_*` for peak-propagation and `chenle02_*` / `MJ_*` for AI images.
- Prefer lossless `.png` for new diagrams; keep vector `.eps` or `.pdf` when available for publication-quality output.
- Markdown files (`README.md`, `AGENTS.md`) should use clear headings, concise bullet lists, and short paragraphs tailored to mathematicians and SPDE users.

## Quality & Validation Guidelines
- Verify every new image opens, renders at suitable resolution for slides/posters, and is not excessively large on disk without need.
- Keep raw data or scripts (when available) near the figures they generate, or referenced from a local `README.md`.
- Check all new links and relative paths in Markdown before committing.

## Commit & Pull Request Guidelines
- Use focused commits with clear messages, e.g. `feat(images): add new SHE peak plots` or `docs(readme): document AI image set`.
- Avoid re-encoding or mass-renaming existing images unless there is a strong reason; explain such changes clearly in the commit message or PR description.
- PRs should briefly state purpose, list key added/modified paths, and note how any newly generated figures were created.

