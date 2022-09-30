---
kind: 🏠 Home
title: Changelog
---
# Clever Components changelog

## [2.0.1](https://github.com/CleverCloud/clever-components-test-ci/compare/2.0.0...2.0.1) (2022-09-30)


### Bug Fixes

* add debug ([8aed3a0](https://github.com/CleverCloud/clever-components-test-ci/commit/8aed3a0932d05ec0f83235148bcc52faac894044))
* add id to release-please action ([b2c3783](https://github.com/CleverCloud/clever-components-test-ci/commit/b2c3783c9500d11c29ae237d0861d8abcb41a5aa))
* debug ([0b6305c](https://github.com/CleverCloud/clever-components-test-ci/commit/0b6305cb4d6f238bba07011e4996a268b2719808))
* debug ([c92b91e](https://github.com/CleverCloud/clever-components-test-ci/commit/c92b91e3eb3e59e877ef7335206a3344cee4f771))
* remove command manifest ([24d720c](https://github.com/CleverCloud/clever-components-test-ci/commit/24d720c35ade1d75fb39db309abe1619462bfa9b))
* use command manifest ([a924d29](https://github.com/CleverCloud/clever-components-test-ci/commit/a924d297e8b6b3bf826e171488832627a6fddc40))

## [2.0.0](https://github.com/CleverCloud/clever-components-test-ci/compare/v1.8.0...2.0.0) (2022-09-30)


### ⚠ BREAKING CHANGES

* remove debug

### Features

* debug github steps ([6c68c83](https://github.com/CleverCloud/clever-components-test-ci/commit/6c68c8398e86680fb2f7beaed87601f712e630c3))
* no v for version tag ([d4c4102](https://github.com/CleverCloud/clever-components-test-ci/commit/d4c41021d727830fff28cae370e158a2ee264be4))
* remove debug ([a51f63e](https://github.com/CleverCloud/clever-components-test-ci/commit/a51f63e59287d74b1c7a130c9772e7fec56a5720))

## [1.8.0](https://github.com/CleverCloud/clever-components-test-ci/compare/v1.7.0...v1.8.0) (2022-09-29)


### Features

* with npm publish ([16e4efc](https://github.com/CleverCloud/clever-components-test-ci/commit/16e4efc0a4033120b80f5dd05a0d09ef0087fd46))

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
