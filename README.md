
# targetprocess-mashup-manifest-loader

Webpack loader to create Targetprocess mashup system configs from single JSON file.

## Usage

```js
// manifest.json
{
    "ShortDescription": "This mashup creates happiness and brings smiles.",
    "CompatibleTpVersion": {
        "Minimum": "3.6.6"
    },
    "Placeholders": [
        "footerplaceholder"
    ]
}
```

```js
require('targetprocess-mashup-manifest-loader!./manifest.json');
// will produce
// ./manifest.baseinfo.json
// ./manifest.cfg
```

## License

MIT (http://www.opensource.org/licenses/mit-license.php)
