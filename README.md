<!-- DOCTOC SKIP -->

# solidity-docgen-template
A template for [solidity-docgen](https://github.com/OpenZeppelin/solidity-docgen)

To add this template as a submodule execute the following commands:
```bash
git submodule add git@github.com:tzapu/solidity-docgen-template.git docs/templates
npm i -D doctoc@git+ssh://git@github.com:thlorenz/doctoc.git#master
npm i -D solidity-docgen    
```

Add `docs` to your `package.json` scripts as pictured
```
"scripts": {
    "docs": "solidity-docgen --solc-module solc-0.8.6 -t docs/templates && doctoc ./docs/ --maxlevel 3",
},
```

Run the docs generating script
```bash
yarn docs
```
