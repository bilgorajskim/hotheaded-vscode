# How to contribute<br/><span style="font-size: 0.4em">Actually, how to build the project</span>

## Preparations

1. Have Node.JS and `npm` installed.
2. Run `npm install` in this project.
3. Edit the deceleration file for the `node-speaker` package to actually work.
	1. Open [`node_modules/speaker/index.d.ts`](node_modules/speaker/index.d.ts).
	2. Write `declare` in front of the namespace and class.
	3. On the last line, change `export`**`s`** to `export`.

## Building, Packaging, and Installing

1. Run `npx vsce package` to build and package the extension.
2. You should now have a `.vsix` file in your top directory. Install it by
   hitting `F1` and typing `install from VSIX` and then selecting the new file.
3. You might have to restart VS Code for the install to take effect.

## Development

If you actually want to help develop you can debug the extension jus by hitting
`F5` in VS Code to start the built-in debugger.