# KernelX — Modular Educational Operating System Kernel

**KernelX** is an educational operating-system kernel project developed to explore low-level system programming, kernel architecture, and filesystem implementation through a bootable x86 environment.

The project focuses on modular kernel development, incorporating a Virtual File System (VFS), an in-memory RAMFS backend, TAR/USTAR archive handling, filesystem-related kernel interfaces, and a kernel-resident command shell.

## Core Components

- **Boot and Kernel Initialization** — Establishes the initial execution environment for the kernel.
- **Virtual File System (VFS)** — Provides a common abstraction for filesystem operations.
- **RAMFS** — Implements an in-memory filesystem backend.
- **TAR/USTAR Archive Loader** — Handles archive-based initial filesystem content.
- **Filesystem Interfaces** — Connects filesystem functionality with other kernel components.
- **Kernel-Resident Shell** — Provides an interactive command interface through the `KernelX:/>` prompt.
- **QEMU Validation** — Supports boot and integration testing in an emulated environment.

## Technology Stack

| Category | Technologies |
|---|---|
| Programming Language | C |
| Architecture | x86 (32-bit) |
| Development Environment | Windows, WSL2 |
| Bootloader | GRUB / Multiboot-based boot workflow |
| Filesystem | VFS, RAMFS, TAR/USTAR |
| Emulation | QEMU |
| Build Tools | GCC, GNU Linker |
| Testing | Host-side tests, QEMU boot validation |

## Development and Validation

The project was developed incrementally, with individual kernel and filesystem components tested before integration.

| Validation Activity | Result |
|---|---|
| C compilation and 32-bit ELF linking | Successful |
| VFS host-side tests | Passed |
| RAMFS host-side tests | Passed |
| Nested USTAR test | Passed |
| ISO generation and QEMU boot | Successful |
| Phase 7 test suite | 16 tests passed |

*These results are based on the project's development records and are not independent certification results.*

## Research Paper

The accompanying research paper documents:

- KernelX design and implementation
- Virtual filesystem design
- RAMFS implementation
- TAR/USTAR archive handling
- Development and validation methodology
- Results, limitations, and future enhancements

## Current Scope and Limitations

KernelX is an educational kernel prototype, not a complete general-purpose operating system.

The available implementation record does not establish:

- A complete Ring 3 user-mode process model
- A complete process scheduler
- Persistent block-device filesystem support
- A complete networking stack
- Production-grade security and memory isolation

## Future Enhancements

- User-mode execution and system-call ABI
- Process and thread scheduling
- Virtual memory and paging
- Interrupt and exception handling improvements
- Persistent storage support
- Filesystem permissions and access control
- Expanded automated testing

## References

1. Intel — *Intel 64 and IA-32 Architectures Software Developer's Manual*.
2. GNU GRUB — *Multiboot2 Specification*.
3. Linux Kernel Documentation — *Virtual File System*.
4. Linux Kernel Documentation — *Ramfs, Rootfs and Initramfs*.
5. QEMU — *System Emulation User's Guide*.
6. A. S. Tanenbaum and H. Bos — *Modern Operating Systems*.
7. R. Love — *Linux Kernel Development*.

## Author

**Chethana Sri**  
Department of Computer Technology  
Madras Institute of Technology, Anna University  
Chennai, India

---

*KernelX — Understanding operating systems by building one subsystem at a time.*
