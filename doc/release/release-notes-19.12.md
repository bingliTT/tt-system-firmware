# v19.12.0

> This is a working draft for the up-coming 19.12.0 release.

We are pleased to announce the release of TT System Firmware version 19.12.0 🥳🎉.

Major enhancements with this release include:

## What's Changed

## Wormhole

## Blackhole

### Power & Performance Improvements
- Enable process based V/F curve for p300c

### Ethernet

- Updated Blackhole ERISC FW to v1.12.0
  - Added support for alternative SerDes link speeds (95G, 106G)
  - Reworked runtime link check and recovery logic
    - Replaced recovery branches with an exponential-backoff escalator: SerDes retrain -> full reinit -> bring port down
    - Added port-down auto-recovery via a sustained-sigdet counter; link-from port down now only happens during retrains
  - Refactored eth_api_table so every API has a wrapper that records call count, last call timestamp, and time spent in function

## Grendel

<!-- Subsections can break down improvements by (area or board) -->
<!-- UL PCIe -->
<!-- UL DDR -->
<!-- UL Ethernet -->
<!-- UL Telemetry -->
<!-- UL Debug / Developer Features -->
<!-- UL Drivers -->
<!-- UL Libraries -->

<!-- Performance Improvements, if applicable -->
<!-- New and Experimental Features, if applicable -->
<!-- External Project Collaboration Efforts, if applicable -->
<!-- Stability Improvements, if applicable -->
<!-- Security vulnerabilities fixed? -->
<!-- API Changes, if applicable -->
<!-- Removed APIs, H3 Deprecated APIs, H3 New APIs, if applicable -->
<!-- New Samples, if applicable -->
<!-- Other Notable Changes, if applicable -->
<!-- New Boards, if applicable -->

## Migration guide

An overview of required and recommended changes to make when migrating from the previous v19.11.0 release can be found in [19.12 Migration Guide](https://github.com/tenstorrent/tt-system-firmware/tree/main/doc/release/migration-guide-19.12.md).

## Full ChangeLog

The full ChangeLog from the previous v19.11.0 release can be found at the link below.

https://github.com/tenstorrent/tt-system-firmware/compare/v19.11.0...v19.12.0
