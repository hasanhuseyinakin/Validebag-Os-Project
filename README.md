# Validebağ-OS: A Linux Distribution Built from Scratch



As computers have become central to modern life, Linux has emerged as a key open-source platform. However, its early interfaces were often non-user-friendly and offered limited application support, creating barriers for students and newcomers. Existing education-focused distributions frequently faced issues with older or low-spec hardware, high system requirements, and lack of Turkish documentation, leaving many students without an accessible platform to learn. To address this, I started building Validebağ-OS from scratch as my capstone project, following the principles of Linux From Scratch (LFS). The project reconstructs the system layer by layer, from the Linux kernel and GNU toolchain to essential packages, providing full transparency and control over the operating system. The aim is to create a minimal, high-performance system free from unnecessary software and telemetry, while remaining fully compatible with modest hardware. Currently, the project has completed the toolchain compilation, and over 90 essential packages—including Python, Bash, GCC, Coreutils, systemd, and many more—are being integrated in an isolated build environment. These packages form the foundation of the system and will later support education modules, CLI tools, and interactive learning environments. Although this is an early alpha stage, the eventual goal is to provide Turkish documentation and interactive modules for HTML, Bash, C, C++, and Python, a layer translating classic Linux commands into Turkish, optimized performance with lower RAM and CPU usage, and faster boot times than existing education distributions, and unique tools such as a Bash/JSON-based download manager. The project’s visual identity draws inspiration from Validebağ Grove’s central 300-year-old plane tree, symbolizing deep roots, resilience, and continuous growth. Validebağ-OS is designed not just as a technical achievement, but as a contribution to digital independence in education, reducing reliance on foreign technologies, and serving the open-source community. While the current version mainly consists of the toolchain and foundational packages, subsequent releases will gradually incorporate all planned features and education modules. Since this is an early alpha (0.1 version), some features are incomplete or unstable. Users are encouraged to test in a virtual machine and provide feedback via our Reddit community: https://www.reddit.com/r/ValidebagOsCommunity/





The following packages and their upstream maintainers are acknowledged for their work, forming the foundation of Validebağ‑OS:


-Python‑3.13.7: Python core developers / Python Software Foundation (CPython upstream)

-XML‑Parser‑2.47: Perl XML::Parser upstream (Perl community)

-acl‑2.3.2: GNU ACL utilities (GNU Project)

-attr‑2.5.2: GNU Attr utilities (GNU Project)

-autoconf‑2.72: GNU Autoconf (GNU Project)

-automake‑1.18.1: GNU Automake (GNU Project)

-bash‑5.3: Bash shell, created by Brian Fox / maintained by Chet Ramey and the GNU Project

-bc‑7.0.3: GNU bc (GNU Project)

-binutils‑2.45: GNU Binutils (GNU Project)

-bison‑3.8.2: GNU Bison (GNU Project)

-bzip2‑1.0.8: bzip2 maintainer (GNU‑compatible, original by Julian Seward)

-coreutils‑9.7: GNU Core Utilities (GNU Project)

-dejagnu‑1.6.3: DejaGnu testing framework (GNU Project)

-diffutils‑3.12: GNU Diff Utilities (GNU Project)

-e2fsprogs‑1.47.3: e2fsprogs upstream (Ted T’so et al.)

-elfutils‑0.193: Elfutils upstream (GNU Project)

-expat‑2.7.1: Expat XML parser (MIT License, James Clark / Expat project)

-expect‑5.45.4: Expect test automation tool (Don Libes, public domain)

-file‑5.46: File type recognizer (original by Ian Darwin et al.)

-findutils‑4.10.0: GNU Find Utilities (GNU Project)

-flex‑2.6.4: Flex lexical analyser (Free Software Foundation)

-flit_core‑3.12.0: Flit packaging tool (Python packaging community)

-gawk‑5.3.2: GNU Awk (GNU Project)

-gcc‑15.2.0: GNU Compiler Collection (GNU Project)

-gdbm‑1.26: GNU GDBM (GNU Project)

-gettext‑0.26: GNU Gettext (GNU Project)

-glibc‑2.42: GNU C Library (GNU Project)

-gmp‑6.3.0: GNU Multiple Precision arithmetic library (GNU Project)

-gperf‑3.3: GNU Perfect hash generator (GNU Project)

-grep‑3.12: GNU Grep (GNU Project)

-groff‑1.23.0: GNU Groff (GNU Project)

-grub‑2.12: GNU GRUB bootloader (GNU Project)

-gzip‑1.14: GNU Gzip (GNU Project)

-iana‑etc‑20250807: IANA time zone and protocols data (IANA / community)

-inetutils‑2.6: GNU Inetutils (GNU Project)

-intltool‑0.51.0: GNU Intltool (GNU Project)

-iproute2‑6.16.0: IPRoute2 utilities (original by Alexey Kuznetsov et al.)

-jinja2‑3.1.6: Jinja2 templating engine (Pallets Projects)

-kbd‑2.8.0: Linux console utilities (Kbd project)

-kmod‑34.2: Kmod kernel module utilities (kernel.org community)

-less‑679: Less pager (less project)

-lfs‑bootscripts‑20250827: LFS bootscripts (Linux From Scratch community)

-libcap‑2.76: Linux capabilities library (libcap project)

-libffi‑3.5.2: libffi foreign function library (Libffi project)

-libpipeline‑1.5.8: Libpipeline (Libpipeline project)

-libtool‑2.5.4: GNU Libtool (GNU Project)

-libxcrypt‑4.4.38: libxcrypt library (libxcrypt project)

-linux‑6.16.1: Linux kernel (Linus Torvalds & kernel community)

-lz4‑1.10.0: LZ4 compression (LZ4 open source project)

-m4‑1.4.20: GNU M4 macro processor (GNU Project)

-make‑4.4.1: GNU Make (GNU Project)

-man‑db‑2.13.1 & man‑pages‑6.15: Manual page utilities (man‑db project / linux docs)

-markupsafe‑3.0.2: MarkupSafe templating utility (Pallets Projects)

-meson‑1.8.3: Meson build system (Meson project)

-mpc‑1.3.1 & mpfr‑4.2.2: GNU MPC / MPFR maths libraries (GNU Project)

-ncurses‑6.5: Ncurses terminal handling (Ncurses project)

-ninja‑1.13.1: Ninja build tool (Ninja project)

-openssl‑3.5.2: OpenSSL cryptography (OpenSSL project)

-packaging‑25.0: Python packaging tools (Python Packaging Authority community)

-patch‑2.8: GNU Patch (GNU Project)

-perl‑5.42.0: Perl programming language (Perl community)

-pkgconf‑2.5.1: pkgconf configuration tool (pkgconf project)

-procps‑ng‑4.0.5: Procps‑ng system utilities (Procps‑ng project)

-psmisc‑23.7: Psmisc process utilities (Psmisc project)

-python‑3.13.7‑docs‑html: Python docs (Python community)

-readline‑8.3: GNU Readline (GNU Project)

-sed‑4.9: GNU Sed (GNU Project)

-setuptools‑80.9.0: Setuptools Python packaging (Python Packaging Authority community)

-shadow‑4.18.0: Shadow password utilities (Shadow project)

-sysklogd‑2.7.2: System logging utilities (Klogd project)

-systemd‑257.8 & systemd‑man‑pages‑257.8: systemd system manager (systemd project)

-sysvinit‑3.14: SysV init utilities (SysVinit project)

-tar‑1.35: GNU Tar (GNU Project)

-tcl8.6.16: Tcl scripting language (Tcl community)

-texinfo‑7.2: GNU Texinfo (GNU Project)

-tzdata‑2025b: Time zone database (IANA / community)

-udev‑lfs‑20230818: Udev scripts (LFS community)

-util‑linux‑2.41.1: Util‑Linux project (util-linux project)

-vim‑9.1.1629: Vim text editor (Bram Moolenaar & Vim community)

-wheel‑0.46.1: Python wheel packaging (Python Packaging Authority community)

-xz‑5.8.1: XZ Utils (XZ Utils project)

-zlib‑1.3.1: zlib compression (Jean‑loup Gailly & Mark Adler)

-zstd‑1.5.7: Zstandard compression (Facebook open source)
