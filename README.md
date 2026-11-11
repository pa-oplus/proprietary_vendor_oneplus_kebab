# OnePlus 8T (kebab) vendor — Paranoid Android

Unified proprietary output for `vendor/oneplus/kebab`, branch `calcite`.
Contains 2,550 already-processed files from the matching TheMuppets lineage-24.0
kebab and sm8250-common repositories. Source revisions and generator provenance
are recorded in SOURCE_PROVENANCE.json; merged metadata is preserved in
provenance/proprietary-files.txt.

The device tree strictly includes this single product/board output as of
`pa-oplus/device_oneplus_kebab` commit `1a89a8a`. Its actual single extractor
regenerates all four build files byte-for-byte with 777 unique named Blueprint
modules. All 2,550 blob contents match the references and all 32 allowed pins
match. No binary/config/APK fixup pass was replayed.

The device supplies the fingerprint shim and selects existing PA camera/crypto
vendor compatibility modules. Vendor perf uses the stock OnePlus HIDL 2.2 stack;
its service/config ownership and missing manifest declaration are handled in the
device tree. OnePlus powerhint.xml remains the sole explicitly selected file.
The intentional ODM fingerprint override and blob bytes are preserved.

This remains an untested integration baseline. PA's system AIDL perf2 clients
require reconciliation with the stock HIDL backend. Forty-two legacy HAL records,
full source/variant/symbol compatibility, kernel/header integration, target VINTF
matrices/SELinux, product build and hardware validation remain pending. The former
full PA checkout is unavailable; source installation into its replacement is pending.

Detailed checks and integration boundaries:
https://github.com/pa-oplus/device_oneplus_kebab/blob/calcite/docs/vendor-consolidation.md
