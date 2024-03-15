# ChangeLog

* All notable changes to the "Windmillcode Snippets 0" extension pack will be documented in this file.

* Version updates will be based on vscode relesases
on every vscode update a new version will be release

* the software version extends the vscode patch version by 3 zeros giving us
1000 possible updates before there is an update to vscode and extends back to zero

* you would have to check the CHANGELOG for any breaking, (major), minor or patched updates which will be denoted respectively



## [1.85.1000] - 2023-12-27
* Extension made available to the public ready for use

## [1.85.1001] - 2023-12-28
* [CHANGE] Removed angular jasmine toHaveBeenCalled just use angular jasmine toHaveBeenCalledWith

## [1.85.1002] - 2024-01-02
* update snippets to support wmlanimate from the wml-components-base library


## [1.85.1003] - 2024-01-19
* update in flask route snippet for quicker code

## [1.86.1000] - 2-10-2024
* added arrange act assert comments in flask route test case generator

## [1.86.1001] - 2-19-2024
* updated color var support for the my-rgb-to-filter fn

## [1.86.1002] - 2-21-2024
* update scss.json wml-spacing to only use css variables

## [1.86.2000] - 2-21-2024
* [FIX] updated scss.json wml-spacing put number outside parentheses

## [1.87.0]  - 3-3-2024

### Changes to `typescript.json`
- In the TypeScript snippet, the constructor parameter name was changed from `params` to `props`.
- Correspondingly, the variable `origParams` was renamed to `origProps` to reflect the change in the constructor parameter.
- The `Object.assign` method now uses `origProps` instead of `origParams`.

### Changes to `typescriptreact.json`
- Added a new snippet under the "class" key:
  - The snippet defines an exported class with a constructor that accepts `props` of type `Partial<$1>`.
  - Inside the constructor, `props` is converted to entries, filtered to exclude keys starting with 'param', and then used to assign values to the class instance.
  - A description was added for the snippet: "Creates a class with a filtered constructor".


## [1.87.1000] - 3-10-2024
* [PATCH] Updated the 'data' field in the request body from a string to an empty dictionary in the Python snippets configuration.

## [1.87.2000] - 3-15-2024

* [UPDATE] Changed constructor parameter name from `props` to `params` in TypeScript snippets.
* [PATCH] Updated object assignment to use `origParams` instead of `origProps` in TypeScript snippets.
* [UPDATE] Changed constructor parameter name from `props` to `params` in TypeScript React snippets.
* [PATCH] Updated object assignment to use `origParams` instead of `origProps` in TypeScript React snippets.
