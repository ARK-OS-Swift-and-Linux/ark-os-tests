# ARK-OS Test Suites

## Overview

The `tests/` repository contains automated testing frameworks, integration harnesses, and virtual machine boot verification suites for ARK-OS.

---

## Directory Organization

- `unit/` - Unit test suites for individual first-party libraries (`libark`), system runtime routines, and shell utilities.
- `integration/` - Cross-component test scenarios validating IPC mechanisms, virtual filesystem interactions, and service orchestration.
- `boot/` - QEMU-driven automated smoke and regression test harnesses verifying kernel startup, ramdisk extraction, PID 1 handoff, and console output.

---

## Testing Principles

- Test cases must assert clear, observable behavior rather than mirroring internal implementation details.
- Boot tests must execute non-destructively in emulator environments (e.g., QEMU) with verifiable timeouts and headless execution modes.
- Never run build or test commands without explicit user authorization per [AGENTS.md](file:///home/aarav/repo/arkos/AGENTS.md) Section 6.

---

## License

This repository is licensed under the Apache License, Version 2.0. See [LICENSE](file:///home/aarav/repo/arkos/tests/LICENSE) for the full license text.
