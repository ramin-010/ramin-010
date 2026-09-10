# Rinkal Kumar (Ramin)

Backend and developer-tooling work in Node and TypeScript. I like the unglamorous parts — streams,
file pipelines, protocol edge cases, the bug that only shows up on the third reconnect.

Full-stack developer at I-3 Integrated Co., Chandigarh.

## Open-source contributions

Bugs I found by reading the source, reproduced with a failing test, and fixed.

| Project | Contribution | Status |
|---|---|---|
| [fastmcp](https://github.com/punkpeye/fastmcp) | [#366](https://github.com/punkpeye/fastmcp/pull/366) — `embedded()` silently dropped resource contents when a template's `load()` returned an array, producing a response that failed MCP schema validation | Merged, shipped in v4.20.9 |
| [hocuspocus](https://github.com/ueberdosis/hocuspocus) | [#1155](https://github.com/ueberdosis/hocuspocus/pull/1155) — an `onLoadDocument` hook returning the document it was handed made the server encode the whole document and apply it back to itself, on the first connection to every document | Merged |
| [hocuspocus](https://github.com/ueberdosis/hocuspocus) | [#1157](https://github.com/ueberdosis/hocuspocus/pull/1157) — a document created for a load that threw was never destroyed, leaking a `Y.Doc` and an Awareness timer per rejected connection | Merged |
| [fastmcp](https://github.com/punkpeye/fastmcp) | [#369](https://github.com/punkpeye/fastmcp/pull/369) — the documented ping default for HTTP streaming never applied, because it keyed off a field no transport sets | Open |
| [sharp](https://github.com/lovell/sharp) | [#4602](https://github.com/lovell/sharp/pull/4602) — `JxlOptions` did not declare the animation options `jxl()` actually accepts | Open |
| [ioredis](https://github.com/redis/ioredis) | [#2187](https://github.com/redis/ioredis/pull/2187) — a failed auto-resubscribe after reconnect became an unhandled rejection, ending the process even with an error handler registered | Open |

## Things I've built

**[Upfly](https://github.com/ramin-010/upfly)** — file-handling middleware for Node APIs.
A custom Multer storage engine that streams uploads through Sharp and on to S3, GCS or Cloudinary,
with a fallback stream that preserves the original if the transform fails. Published on npm.

**[Upfly for VS Code](https://github.com/ramin-010/VS-Code-Extension-Upfly-)** — drop an image into a
watched folder and it converts, uploads, and returns a CDN URL. File-stability polling, loop
prevention and a git-tracked-file guard, because the naive version corrupts half-written files.

**[ReCollect](https://github.com/ramin-010/ReCollect)** — a collaborative workspace built on Yjs CRDTs
with a custom Hocuspocus WebSocket server, plus multi-model AI routing across Gemini, OpenAI, Groq and
Cohere. The most technically involved thing I've built, and where most of my Redis, BullMQ and
WebSocket experience comes from.

## Stack

TypeScript · JavaScript · Node · Express · Next.js · React · PostgreSQL · MongoDB · Redis · BullMQ ·
WebSockets · Yjs · Sharp · AWS S3 · Cloudinary · GCS

B.Tech CSE, Rayat Bahra University, 2026.

Reach me at rinkalkumar737@gmail.com · [LinkedIn](https://www.linkedin.com/in/rinkal-kumar-46130a329/) · [npm](https://www.npmjs.com/~ramin-010)
