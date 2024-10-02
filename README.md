# sublime-text-jsdoc-snippets

Some snippet definitions for ST4 to sprinkle TS-flavor JSDoc in a breeze

![Demo gif](https://github.com/user-attachments/assets/322b39a5-5563-4217-8304-2c4c2b30b0d6)

## Installing

1. Clone the directory.
2. Symlink the `snippets` directory and the `*.sublime-keymap` file into Sublime Text's `Users` package directory. Naming does not matter.

You can find the location to the package directory from Sublime Text via the command **Preferences: Browse Packages**.

### Recommended settings

You may need to patch your JS/TS(X)-specific settings accordingly for these snippet to work. See the files in the project root. Again, you can open the preference file via the command **Preferences: Settings &ndash; Syntax Specific**.

## Implemented features

* In code: Type `@` and select a snippet. For example, `@type` inserts `/** @type {...} */` and place the caret in the blank for you.
* In comment blocks: In addition to Sublime Text's built-in JSDoc snippets, these snippets save more keystrokes. For example, `@param` inserts `@param {any} foo`.
* TS directives: Type `@ts-` to insert directives of TypeScript. For example `// @ts-ignore`.

I only implement features that the TypeScript compiler recognizes, summarized in [this document](https://hackmd.io/@q/jsdoc-typescript-ref). This is lame but let us face the reality.
