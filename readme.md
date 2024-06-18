# UserTS
This is a project attempting to allow userscripts to be created using modern syntax.

## Why parcel?
It was the first bundler that I got working to output a valid userscript, esbuild would strip out the metadata block, which I can't fix without writing a plugin due to esbuild's fundemental design.

## Naming
UserTS is named after the conventional extension of a userscript, `.user.ts`.