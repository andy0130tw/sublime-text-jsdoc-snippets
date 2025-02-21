# sublime-text-jsdoc-snippets

Some snippet definitions for ST4 to sprinkle TS-flavor JSDoc in a breeze

![Demo gif](https://github.com/user-attachments/assets/322b39a5-5563-4217-8304-2c4c2b30b0d6)

## Installing

1. Clone this repository.
2. Symlink the `snippets` directory and the `*.sublime-keymap` file into Sublime Text's `Users` package directory. Naming does not matter. Do not symlink the project root repository, as that would include some `.sublime-settings` files that are meant to be patched manually.

You can find the location to the package directory from Sublime Text via the command **Preferences: Browse Packages**.

### Recommended settings

You may need to patch your JS/JSX-specific settings accordingly for these snippet to work, especially when [LSP-TypeScript][lsp-typescript] is active. See the files in the project root. Again, you can open the preference file via the command **Preferences: Settings &ndash; Syntax Specific**.

[lsp-typescript]: https://github.com/sublimelsp/LSP-typescript/

## Implemented features

* JSDoc in JS/JSX code: Type `@` in most places and select a snippet. For example, `@type` inserts `/** @type {...} */` and place the caret in the blank for you.
* In comment blocks: In addition to Sublime Text's built-in JSDoc snippets, these snippets save more keystrokes. For example, `@param` inserts `@param {any} foo`.
* TS directives: Type `@ts-` in JS/TS **comments** to insert directives of TypeScript. For example, type `// @` to insert `// @ts-ignore`.
* TS [triple-slash directives][ts-triple-slash-directive]: Type a triple-slash to insert a `<reference ... />` directive by path, name, lib, etc.

[ts-triple-slash-directive]: https://www.typescriptlang.org/docs/handbook/triple-slash-directives.html

I only implement features that the TypeScript compiler v5 recognizes, summarized in [this document][my-hackmd-ref]. This is lame but let us face the reality.

[my-hackmd-ref]: https://hackmd.io/@q/jsdoc-typescript-ref
