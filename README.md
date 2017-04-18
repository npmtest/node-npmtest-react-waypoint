# npmtest-react-waypoint

#### test coverage for  [react-waypoint (v6.0.0)](https://github.com/brigade/react-waypoint)  [![npm package](https://img.shields.io/npm/v/npmtest-react-waypoint.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-react-waypoint) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-react-waypoint.svg)](https://travis-ci.org/npmtest/node-npmtest-react-waypoint)

#### A React component to execute a function whenever you scroll to an element.

[![NPM](https://nodei.co/npm/react-waypoint.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/react-waypoint)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-react-waypoint/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-react-waypoint/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-react-waypoint/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-react-waypoint/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-react-waypoint/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-react-waypoint/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-react-waypoint/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-react-waypoint/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-react-waypoint/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-react-waypoint/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-react-waypoint/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-react-waypoint/build/test-report.html](https://npmtest.github.io/node-npmtest-react-waypoint/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-react-waypoint/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-react-waypoint/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-react-waypoint/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-react-waypoint/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-react-waypoint/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-react-waypoint/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-react-waypoint/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-react-waypoint/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Brigade Engineering"
    },
    "bugs": {
        "url": "https://github.com/brigade/react-waypoint/issues"
    },
    "dependencies": {
        "consolidated-events": "^1.0.1"
    },
    "description": "A React component to execute a function whenever you scroll to an element.",
    "devDependencies": {
        "@types/react": "^15.0.21",
        "babel-cli": "^6.23.0",
        "babel-core": "^6.23.1",
        "babel-loader": "^6.4.0",
        "babel-plugin-add-module-exports": "^0.2.1",
        "babel-plugin-transform-react-jsx": "^6.23.0",
        "babel-preset-es2015": "^6.22.0",
        "eslint": "^3.17.1",
        "eslint-config-brigade": "^3.2.1",
        "eslint-plugin-react": "^6.10.0",
        "in-publish": "^2.0.0",
        "jasmine-core": "^2.1.3",
        "karma": "^1.5.0",
        "karma-chrome-launcher": "^2.0.0",
        "karma-cli": "^1.0.1",
        "karma-firefox-launcher": "^1.0.1",
        "karma-jasmine": "^1.1.0",
        "karma-webpack": "^2.0.3",
        "prop-types": "^15.5.4",
        "react": "^15.5.3",
        "react-dom": "^15.5.3",
        "rimraf": "^2.6.1",
        "safe-publish-latest": "^1.1.1",
        "webpack": "^2.3.3"
    },
    "directories": {},
    "dist": {
        "shasum": "a14c8cb1305bfdf7160ace4f8a087d6c7f745639",
        "tarball": "https://registry.npmjs.org/react-waypoint/-/react-waypoint-6.0.0.tgz"
    },
    "gitHead": "b23770d57fa66b4e20eeb3e8d80fa60d85135f36",
    "homepage": "https://github.com/brigade/react-waypoint",
    "keywords": [
        "react",
        "component",
        "react-component",
        "scroll",
        "onscroll"
    ],
    "license": "MIT",
    "main": "build/waypoint.js",
    "maintainers": [
        {
            "name": "brigade"
        },
        {
            "name": "jmeas"
        },
        {
            "name": "lencioni"
        },
        {
            "name": "trotzig"
        }
    ],
    "name": "react-waypoint",
    "optionalDependencies": {},
    "peerDependencies": {
        "react": "^0.14.0 || ^15.0.0",
        "prop-types": "^15.0.0"
    },
    "repository": {
        "type": "git",
        "url": "git+https://github.com/brigade/react-waypoint.git"
    },
    "scripts": {
        "build": "npm run clean && babel src/ -d build/",
        "check-changelog": "expr $(git status --porcelain 2>/dev/null| grep \"^\\s*M.*CHANGELOG.md\" | wc -l) >/dev/null || (echo 'Please edit CHANGELOG.md' && exit 1)",
        "check-only-changelog-changed": "(expr $(git status --porcelain 2>/dev/null| grep -v \"CHANGELOG.md\" | wc -l) >/dev/null && echo 'Only CHANGELOG.md may have uncommitted changes' && exit 1) || exit 0",
        "clean": "rimraf build",
        "lint": "eslint . --ext .js,.jsx",
        "postversion": "git commit package.json CHANGELOG.md -m \"Version $npm_package_version\" && npm run tag && git push && git push --tags && npm publish",
        "prepublish": "in-publish && safe-publish-latest && npm run build || not-in-publish",
        "pretest": "npm run --silent lint",
        "preversion": "npm run test && npm run check-changelog && npm run check-only-changelog-changed",
        "tag": "git tag v$npm_package_version",
        "test": "npm run testonly",
        "testonly": "karma start --single-run",
        "testonly:watch": "karma start --no-single-run"
    },
    "types": "index.d.ts",
    "version": "6.0.0"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
