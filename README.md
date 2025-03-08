# oxlint-named-enum-js-bug

Oxlint reports an error from `import/named` when importing an enum into a `.js` file

```
  × eslint-plugin-import(named): named import "Events" not found
   ╭─[jsFile.js:1:9]
 1 │ import {Events} from "./enums";
   ·         ──────
 2 │
   ╰────
  help: does "./enums" have the export "Events"?
```

It does not report such an error when importing an enum into a `.ts` file. 
