# OnePlus 8T (kebab) vendor — Paranoid Android

Unified proprietary vendor baseline for `vendor/oneplus/kebab`, branch `calcite`.
Contains 2,550 proprietary files from the matching TheMuppets `lineage-24.0`
kebab and sm8250-common repositories. Exact commits and generation provenance
are recorded in SOURCE_PROVENANCE.json; the merged input list is preserved in
provenance/proprietary-files.txt.

Build files were regenerated for one kebab producer with 777 unique named
Blueprint modules. Blob contents, pins and existing Lineage processing are
preserved; no binary/config/APK fixup pass was rerun. Existing generated files
from the two inputs were not concatenated.

This is an integration baseline, not a tested PA release. The fingerprint shim,
camera/crypto provider variants, intentional fingerprint VINTF override, OnePlus
perf/source ownership and remaining vendor/legacy declarations require final
integration. PA product/vendor includes have not been activated by publication.
Kernel/header, complete Soong/VINTF/SELinux and hardware validation remain pending.

Device configuration and the detailed consolidation plan:
https://github.com/pa-oplus/device_oneplus_kebab/tree/calcite
