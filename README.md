<!-- DOCTOC SKIP -->

# solidity-docgen-template
a template for solidity-docgen

Execute the following commands
```bash
git submodule add git@github.com:tzapu/solidity-docgen-template.git docs/templates
npm i -D doctoc@git+ssh://git@github.com:thlorenz/doctoc.git#master
npm i -D solidity-docgen    
```

Add `docs` to your `package.json` scripts like pictured
```
"scripts": {
    "docs": "solidity-docgen --solc-module solc-0.8.6 -t docs/templates && doctoc ./docs/ --maxlevel 3",
},
```

Run the docs generating script
```bash
yarn docs
```
