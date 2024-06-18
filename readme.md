# UserTS
This is a project attempting to allow userscripts to be created using modern syntax.

## Why parcel?
It was the first bundler that I got working to output a valid userscript, esbuild would strip out the metadata block, which I can't fix without writing a plugin due to esbuild's fundemental design.

## Usage
```sh
git clone https://github.com/WiDuMu/userts.git
cd userts
```
Clone the repo, then run using either npm or bun:

### NPM
```sh
npm i
npm run build
```
### Bun
```sh
bun i
bun run build
```
This will create a `/dist` directory containing a `user.js` file, which is the final output. From here, you should be able to install dependencies and import them in your `user.ts` file. It is recommended to read the [metadata block](https://violentmonkey.github.io/api/metadata-block/), and [greasemonkey api](https://violentmonkey.github.io/api/gm/) documentation to modify the metadata block for the site you want.
## Naming
UserTS is named after the conventional extension of a userscript, `.user.js`.
