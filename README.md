language-mapping-list
=====================

List of all the known languages in their English and Native name with locales.

There are over 200 languages available in the list.

`$ npm install @subiz/langmap`

Usage:

```
var langmap = require("langmap");

"Native" => English (US)
var native = langmap["en-US"]["nativeName"];
"Native" => ภาษาไทย
var native = langmap["th"]["nativeName"];
"English" => Thai
var native = langmap["th"]["englishName"];

```

### What locales are missing?

```sh
node ./findMissing.js
```

### Note when adding new locales

* Append to the bottom of the file './language-mapping-list.js'. *Do not* add to the middle
* Build the proto in `github.com/subiz/header`: `docker build --progress=plain -t live360vn/protobuild:2.6 .`
