# yaml-utils

[![latest version published to npm](https://badge.fury.io/js/yaml-utils.svg)](https://www.npmjs.com/package/yaml-utils)

CLI tools for converting JSON to YAML and vice versa.

```sh
npm install -g yaml-utils
```

This package provides two `bin` scripts:


### `json2yaml`

YAML is a superset of JSON, so there are lots of ways to convert JSON to YAML.
But one is better than none.

```sh
json2yaml < package.json
```

Results in:

```yaml
name: yaml-utils
version: 1.1.0
description: CLI tools for converting JSON to YAML and vice versa
license: MIT
keywords:
  - cli
  - json
  - yaml
repository: 'git://github.com/chbrown/yaml-utils.git'
homepage: 'https://github.com/chbrown/yaml-utils'
author: Christopher Brown <io@henrian.com>
dependencies:
  js-yaml: ^3.11.0
  optimist: 0.6.1
bin:
  json2yaml: json2yaml
  yaml2json: yaml2json
```


### `yaml2json`

Read in YAML and output JSON.

```sh
yaml2json < package.yaml | jq .
```


## License

Copyright © 2014–2019 Christopher Brown.
[MIT Licensed](https://chbrown.github.io/licenses/MIT/#2014-2019).
