# OnePlus 8T (kebab) vendor — Paranoid Android

Unified output for `vendor/oneplus/kebab`, branch `calcite`. The single extractor
and strict device product/board includes are in pa-oplus/device_oneplus_kebab.

The original 2,550 processed TheMuppets lineage-24.0 files are unchanged. Two pinned
PA common DSP server input files supply the previously missing DSP service/RC.
Their exact input hashes and local source paths are in SUPPLEMENTAL_INPUTS.json;
the original supplemental repository commit metadata is unavailable. Source
provenance and the active merged-list hash are recorded in SOURCE_PROVENANCE.json.

All 2,552 entries regenerate four identical build files with 778 unique named
vendor modules. All 34 allowed pins pass. Original input bytes and supplemental
source bytes match their references. No binary/config/APK fixup pass was replayed.

The device selects stock graphics, alarm, media/WFD and perf without competing
common proprietary imports. Fingerprint/camera/crypto compatibility providers are
selected. Exact PA system perf clients have a HIDL 2.2 fallback for shipping API
30 when no AIDL perf2 service is declared; runtime behavior is untested.

Static legacy HAL resolution is complete in the device tree: 51 records declared,
one unsupported optional Oplus subsystem-radio interface explicitly not selected.
Thirty-four recorded local/reference-source/vendor fragments merge into 109 unique
instances and preserve the intentional fingerprint override. These checks do not
prove that every service registers or works in a built product.

Required source selections and an audio registration patch are prepared. A full
PA source checkout, kernel/header integration, complete module/variant/ABI/linker,
SELinux/matrix, product compilation and hardware tests remain pending. This is an
integration baseline, not a tested or boot-verified release.

Current gates and evidence:
https://github.com/pa-oplus/device_oneplus_kebab/blob/calcite/docs/INTEGRATION_STATUS.md
