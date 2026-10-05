<!-- tyhp-readme:start -->
# tyhpdef/infection-infection

Tyhp type definitions for `infection/infection` `0.35.4`.

```bash
composer require --dev tyhpdef/infection-infection:0.35.4
```

This is a metapackage. Composer also installs `tyhpdef/infection-infection-impl` (type files).
Require **this** name, not `tyhpdef/infection-infection-impl`.

See https://tyhplang.com.

## Maintain `infection/infection`? Ship the types yourself

If you are a Packagist maintainer of `infection/infection`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/infection-infection-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `infection/infection` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/infection-infection": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `infection/infection` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `infection/infection` with a real constraint,
   `"replace": { "tyhpdef/infection-infection": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `infection/infection` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/infection-infection` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
