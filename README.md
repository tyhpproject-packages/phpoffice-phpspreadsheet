<!-- tyhp-readme:start -->
# tyhpdef/phpoffice-phpspreadsheet

Tyhp type definitions for `phpoffice/phpspreadsheet` `5.9.0`.

```bash
composer require --dev tyhpdef/phpoffice-phpspreadsheet:5.9.0
```

This is a metapackage. Composer also installs `tyhpdef/phpoffice-phpspreadsheet-impl` (type files).
Require **this** name, not `tyhpdef/phpoffice-phpspreadsheet-impl`.

See https://tyhplang.com.

## Maintain `phpoffice/phpspreadsheet`? Ship the types yourself

If you are a Packagist maintainer of `phpoffice/phpspreadsheet`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/phpoffice-phpspreadsheet-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `phpoffice/phpspreadsheet` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/phpoffice-phpspreadsheet": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `phpoffice/phpspreadsheet` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `phpoffice/phpspreadsheet` with a real constraint,
   `"replace": { "tyhpdef/phpoffice-phpspreadsheet": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `phpoffice/phpspreadsheet` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/phpoffice-phpspreadsheet` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
