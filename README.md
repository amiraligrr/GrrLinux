# 🐧 GRR Linux

> **A minimalist, bootable Linux distribution built from source — with a personal touch.**

---

## 🌟 About

**GRR Linux** is a custom Linux distribution being built from scratch by **Amirali Granmayeh (amiraligrr)** — a 16-year-old developer, robotics champion, and student from Kerman, Iran.

The mission is simple but ambitious: **create a lightweight, reproducible, and educational Linux system** that boots on x86_64, supports both BIOS and UEFI, and gives anyone the tools to learn how an operating system works — from the bootloader to the shell.

GRR Linux is not just another distro. It's a statement:


---

## 🎯 Vision

GRR Linux aims to be:

- **Minimal** — no bloat, no unnecessary packages. Just the essentials.
- **Reproducible** — anyone can run the build scripts and get the same result.
- **Educational** — every part of the system is documented and understandable.
- **Personal** — it carries the signature of its maker, from the boot screen to the motd.
- **Open** — built in public, open to contributors, feedback, and ideas.

---

## 🚧 Current Status (Version 0.1 — Coming Soon)

We are currently in the **pre-release phase**. Version **0.1** is being prepared and will be published **very soon**. Here's what's in progress:

- **Bootloader**: GRUB 2 with BIOS and UEFI support
- **Kernel**: Custom Linux kernel configuration (minimal, with ext4, squashfs, and networking support)
- **Init System**: A simple PID 1 init written in C / Bash
- **Core Utilities**: BusyBox for a minimal footprint
- **Shell**: Bash / Dash
- **Package Manager**: `grrpkg` — a lightweight tool to install, remove, update, and list packages from a local repository
- **File System**: ext4 / squashfs with overlay for persistence
- **Networking**: DHCP client, wget / curl for basic network operations
- **Text Editors**: Vim and Nano
- **Build System**: Reproducible shell scripts that download, compile, and assemble everything from source
- **Testing**: Boot-tested in QEMU and VirtualBox

Once version 0.1 is released, the ISO will be available for download, along with complete build and usage documentation.

---

## 🌐 Website — Coming Soon

A dedicated website for **GRR Linux** is currently under development and will be launched alongside the first release. It will include:

- Downloads (ISO images)
- Build guides and documentation
- Package repository
- Community section
- Project roadmap

Stay tuned — the link will be shared here as soon as it's live.

---

## 🗺️ Roadmap

Here's what we plan to build after version 0.1:

### Short-Term
- **UEFI + BIOS**: Full support for modern and legacy systems
- **Package Repository**: A local repository for `grrpkg` with community-contributed packages
- **Networking Tools**: DHCP, wget, curl, ping, and basic network utilities
- **Documentation**: Complete guides for building, using, and contributing

### Mid-Term
- **Optional GUI**: A lightweight framebuffer-based GUI (TinyX, DirectFB, or custom)
- **Init System Improvements**: Service management, logging, and startup scripts
- **Cross-Compilation Support**: Build for ARM and other architectures
- **Live USB Creator**: A simple tool to write the ISO to a USB drive

### Long-Term
- **Community Contributions**: Open to developers, testers, and translators
- **Custom Installer**: A simple TUI-based installer for GRR Linux
- **GRR Linux Ecosystem**: Tools, packages, and services built around the distro

> **The long-term vision: a fully functional, minimal, and educational Linux distribution that anyone can build, modify, and learn from.**

---

## 🛠️ Build Instructions

Detailed build instructions will be available in [`docs/BUILD.md`](docs/BUILD.md) once version 0.1 is released.

In short:

1. Run the scripts in `build/scripts/` in order.
2. Download sources, build the kernel, compile BusyBox, create the rootfs, and generate the ISO.
3. The final ISO will be placed in the `iso/` directory.
4. Boot it in QEMU or VirtualBox to test.

---

## 📂 Project Structure
grr-linux/
├── build/
│   ├── scripts/          # Build scripts
│   ├── config/           # Kernel, BusyBox, and GRUB configs
│   └── packages/         # Downloaded source tarballs
├── src/
│   ├── init/             # Custom init source
│   ├── grrpkg/           # Package manager
│   └── etc/              # System configuration files
├── iso/                  # Output ISO images
├── docs/                 # Documentation
└── LICENSE

---

## 🤝 Contributing

GRR Linux is open to contributions, ideas, and feedback.  
Whether you're a developer, tester, translator, or just curious — **you're welcome here.**

Ways to contribute:
- Report bugs and issues
- Suggest features
- Submit pull requests
- Write documentation
- Test the ISO on different hardware
- Spread the word

---

## 📜 License

This project is licensed under the **MIT License** — free to use, modify, and distribute.

---

## 📬 Contact

- **GitHub**: [github.com/amiraligrr](https://github.com/amiraligrr)
- **Email**: `amiralig13899@gmail.com` | `admin@amiraligrr.ir`
- **Personal Website**: [amiraligrr.ir](https://amiraligrr.ir)

---

**GRR Linux — Version 0.1 is coming soon. The website is on the way. Stay tuned.** 🐧🔥
