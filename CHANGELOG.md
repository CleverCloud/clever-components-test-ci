---
kind: 🏠 Home
title: Changelog
---
# Clever Components changelog

## 9.0.0 (2022-07-19)

### ⚠️ BREAKING CHANGES

* `<cc-input-text>`:
    * change default font-family to inherit instead of monospace (BREAKING CHANGE),
    * add CSS Custom Prop to change the `<input>` font-family.
* `<cc-input-number>`:
    * change default font-family to inherit instead of monospace (BREAKING CHANGE),
    * add CSS Custom Prop to change the `<input>` font-family.
* `<cc-toggle>`:
    * rename `--cc-text-transform` to `--cc-toggle-text-transform` (BREAKING CHANGE),
    * add CSS Custom Prop to customize `border-radius`, `font-weight`.
* Introduce a public theme based on a CSS files (BREAKING CHANGE):
    * move `default-theme` (design tokens) from a JavaScript file to a CSS file (BREAKING CHANGE),
    * remove `default-theme` import from all components (BREAKING CHANGE),
    * prefix decision design tokens with `cc-` (BREAKING CHANGE),
    * define default text color using `cc-color-text-default` where necessary (BREAKING CHANGE),
    * define default background colors using `cc-color-bg-default` where necessary (BREAKING CHANGE).
* colors: change color decision names finishing with `-light` to `-weak` (for instance: `cc-color-text-weak`). (BREAKING CHANGE)

### Components

* Replace error state after user action by `cc-toast` notification (`cc-grafana-info`, `cc-tcp-redirection-form`, `cc-env-var-form`).
* New components:
    * `<cc-toaster>`
    * `<cc-toast>`
* `<cc-button>`: add CSS Custom Props to customize `border-radius`, `font-weight` and `text-transform`.

### For devs

* `rollup`:
    * add new plugin `rollup-plugin-styles-assets` to bundle the `default-theme` CSS file.
    * add new property (array) `styles` in `deps-manifest` to specify the hashed name of the `default-theme` CSS file corresponding to a specific version (to be used by the CDN).

...
