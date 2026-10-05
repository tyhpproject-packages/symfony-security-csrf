<!-- tyhp-readme:start -->
# tyhpdef/symfony-security-csrf

Tyhp type definitions for `symfony/security-csrf` `7.4.8`.

```bash
composer require --dev tyhpdef/symfony-security-csrf:7.4.8
```

This is a metapackage. Composer also installs `tyhpdef/symfony-security-csrf-impl` (type files).
Require **this** name, not `tyhpdef/symfony-security-csrf-impl`.

See https://tyhplang.com.

## Maintain `symfony/security-csrf`? Ship the types yourself

If you are a Packagist maintainer of `symfony/security-csrf`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/symfony-security-csrf-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `symfony/security-csrf` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/symfony-security-csrf": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `symfony/security-csrf` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `symfony/security-csrf` with a real constraint,
   `"replace": { "tyhpdef/symfony-security-csrf": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `symfony/security-csrf` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/symfony-security-csrf` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
