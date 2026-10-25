
# DreamcastDroid Native Porting Plan

## Target
- CPU: SH-4
- Operating system: Linux
- Android base: Ice Cream Sandwich (4.0)

## Components to investigate

### Toolchain and ABI
- [ ] Select a Linux-targeting SH-4 cross-compiler
- [ ] Record ELF architecture and ABI requirements
- [ ] Verify endianness, calling conventions, and floating-point ABI

### Android native foundation
- [ ] Investigate SH-4 support in Bionic
- [ ] Port or implement the dynamic linker for SH-4
- [ ] Review system-call and kernel-header assumptions
- [ ] Build compatible native utilities

### Android runtime
- [ ] Audit Dalvik VM architecture assumptions
- [ ] Identify assembly and JIT dependencies
- [ ] Evaluate interpreter-only operation as an initial target
- [ ] Audit JNI libraries and native service dependencies

### Validation
- [ ] Compile a minimal SH-4 Linux executable
- [ ] Validate shared-library loading
- [ ] Test basic process and thread operations
- [ ] Record unresolved dependencies

## Status
Planning only. No Android SH-4 binaries have been built.
