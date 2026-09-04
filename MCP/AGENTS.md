## External Documentation and Reference

When implementation depends on an external API, library, framework, toolchain,
hardware SDK, or unfamiliar behavior, do not rely solely on model memory.

Prefer authoritative or grounded sources in this order:

1. Use Context7 for current library and framework documentation.
2. Use project-specific MCP documentation tools when available.
3. Use DeepWiki to inspect and understand public upstream repositories.
4. Use gh_grep to find examples of APIs being used in real source code.
5. Prefer vendor/project documentation over third-party examples when they conflict.

For embedded development, verify register names, constants, function signatures,
Kconfig options, Devicetree properties, pin assignments, peripheral capabilities,
and MCU-specific behavior against authoritative documentation before implementation.
