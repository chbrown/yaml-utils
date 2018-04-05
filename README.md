# yaml-utils

[![latest version published to npm](https://badge.fury.io/js/yaml-utils.svg)](https://www.npmjs.com/package/yaml-utils)

CLI tools for converting JSON to YAML and vice versa.

This package provides two `bin` scripts:

### `json2yaml`

YAML is a superset of JSON, so there are lots of ways to convert JSON to YAML.
But one is better than none.

    json2yaml < package.json
    > name: scripts
    > version: 0.2.0
    > description: Handy scripts
    > keywords:
    >   - scripts
    > ...

### `yaml2json`

Read in YAML and output JSON.

    cat simple_spec.yaml | yaml2json | jq . > simple_spec.json


## License

Copyright © 2014–2018 Christopher Brown.
[MIT Licensed](https://chbrown.github.io/licenses/MIT/#2014-2018).
