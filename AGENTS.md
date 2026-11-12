# AGENTS.md

This file provides guidance to coding agents (Claude Code, Codex, ...) when working with code in this repository.

This is the GitHub profile repository `erupts/erupts`: `README.md` is rendered on the `erupts` profile page
(the home of the erupt framework, `erupts/erupt`). There is nothing to build or test.

- `README.md` is rendered by GitHub, so only GitHub-flavored Markdown and the HTML subset GitHub allows work
  (no scripts, no external CSS). Preview a change on GitHub.
- `me.svg` is the banner at the top of the README; `stack.svg` is the technology-stack image, currently
  switched off through a Markdown comment (`[//]: # (...)`). Both are hand-written, self-contained SVGs with
  inline `<style>` and CSS animations: keep them free of external fonts, images and scripts, and keep the
  `alt` text in the README and the `aria-label` in the SVG in step with what the image says.
- The Java sample in the README is meant to be valid erupt code (`@Erupt`, `@EruptField`, `@View`, `@Edit`);
  check annotation attributes against the erupt repository when changing it.
