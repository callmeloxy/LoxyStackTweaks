# Changelog

## 1.0.0

### Summary

Initial release of LoxyStackTweaks, a lightweight Fabric mod that safely improves Minecraft item stack sizes through configurable rules.

### Added

* Added automatic normalization for vanilla items that are already stackable but limited to fewer than 64 items
* Added support for stacking empty buckets up to 64
* Added protections for:

  * filled buckets
  * durability-based items
  * potentially unsafe data-based items
* Added configurable whitelist support
* Added configurable blacklist support
* Added `forceToOne` support for items that should never stack
* Added optional compatibility with modded items through allowed namespaces
* Added the configuration file:

  * `config/LoxyStackTweaks.json`
* Added configuration reload commands:

  * `/loxystacktweaks reload`
  * `/lst reload`
* Added safe reload handling for invalid JSON configuration files
* Added English and French translations

### Notes

* Modded compatibility is disabled by default
* Storage items and items containing custom data should be handled carefully using the blacklist or `forceToOne`
* Fabric API is required
