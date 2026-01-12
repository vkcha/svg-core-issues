# @vkcha/svg-core — Issue Tracker

This repository is **issues-only** for [`@vkcha/svg-core`](https://www.npmjs.com/package/@vkcha/svg-core).  
The source code lives in a private monorepo, so this repo contains **no implementation code**.

- Docs / homepage / demo: https://vkcha.com
- NPM: https://www.npmjs.com/package/@vkcha/svg-core

## What to file here
- Bug reports
- Feature requests
- Documentation requests
- Performance problems
- Usage questions (or use Discussions if enabled)

## Before you submit
Please include:

- Package version (`@vkcha/svg-core`):
- Browser + OS:
- Expected behavior:
- Actual behavior:
- Minimal reproduction (code snippet or a small repo link):
- Console errors / screenshots (if relevant):
- If the problem is performance-related, include: node count, typical SVG fragment size, and whether culling is enabled.

## Minimal reproduction template

import { SvgCore, Node } from "@vkcha/svg-core";

const svg = document.querySelector("#canvas") as SVGSVGElement;
const core = new SvgCore(svg);

core.setNodes([
  new Node({
    id: "node-1",
    x: 0,
    y: 0,
    fragment: `<rect width="120" height="60" fill="#111827" />`,
  }),
]);
