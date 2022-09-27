# [1.3.0](https://github.com/CleverCloud/clever-components-test-ci/compare/1.2.4...1.3.0) (2022-09-20)


### Bug Fixes

* fix ([f04c35b](https://github.com/CleverCloud/clever-components-test-ci/commit/f04c35b633f16b469bab67cb80e3edb92ecfd83c))
* **readme:** fix readme ([f1374d9](https://github.com/CleverCloud/clever-components-test-ci/commit/f1374d9091d2e4ebaec885c5052355e93c738052))


### Features

* **readme:** feat readme ([812496e](https://github.com/CleverCloud/clever-components-test-ci/commit/812496e1f2b4df7ffe1af3e6c845684e8a6dd300)), closes [#5](https://github.com/CleverCloud/clever-components-test-ci/issues/5)

## [1.2.4](https://github.com/CleverCloud/clever-components-test-ci/compare/1.2.3...1.2.4) (2022-09-20)


### Bug Fixes

* test fix ([50dd1b3](https://github.com/CleverCloud/clever-components-test-ci/commit/50dd1b3a47b0b2c03a9ed47c3c01869baca7c450))

## [1.2.3](https://github.com/CleverCloud/clever-components-test-ci/compare/1.2.2...1.2.3) (2022-09-20)


### Bug Fixes

* remove params from semantic-release/git ([362cd5f](https://github.com/CleverCloud/clever-components-test-ci/commit/362cd5f4ad452c0426cdb112e2ef05da5003a375))


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
