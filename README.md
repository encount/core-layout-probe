# core-layout-probe
A responsive AngularJS layout component for a simple, yet not completely trivial, Web-app layout that works well on both small (mobile) and larger screens.  An important feature is its use of iScroll 5.x, through [angular-iscroll-probe](https://github.com/OnLiveResearch/core-layout-probe), to support fixed-position headers and footers without using the CSS `position: fixed` formatting instruction which is not well supported on older Android (<= 4.1.2 ?) and iOS (<= 8.x) versions.  

## Install

Install the [core-layout-probe NPM package](https://www.npmjs.com/package/core-layout-probe)
```bash
# With NPM:
npm install --save core-layout-probe
# With Yarn, which I prefer:
yarn add core-layout-probe
```

Or, to check out a development version, start by cloning the repository, by
```bash
git clone git@github.com:OnLiveResearch/core-layout-probe.git
```
Then, install the necessary dependencies:
```bash
cd core-layout-probe/
yarn install    # Or: npm install
```
After that, you should have a `dist` directory with a subdirectory named `lib`:
```
dist/
├── lib
│   └── core-layout.js
└── scss
    ├── _core-drawers.scss
    ├── _core-modal.scss
    ├── _core-responsive.scss
    ├── _core.scss
    └── _core-variables.scss
```

### Build

To rebuild the library, run
```bash
yarn build         # Or `yarn watch` (to rebuild on every file change).
```

To build the examples, run
```bash
yarn build-examples  # Or, `npm run-script build-examples`.
```


## Demo
You may have a look at an Angular [demo app](https://onliveresearch.github.io/core-layout-probe/examples/) that shows how you can use this `core-layout-probe` module.

### Building the Demo (`examples/`)
Please note that if you don't plan on changing the demo and testing new stuff, there's no need to compile it yourself; you can just visit the [demo app](https://onliveresearch.github.io/core-layout-probe/examples/).
