# 🧬 Ghostty Configuration for Bioinformatics

A customized **Ghostty** terminal configuration optimized for bioinformatics workflows, data analysis, and sequence alignment on macOS.

## ⚡️ Overview

This configuration is designed to balance **aesthetics** (Catppuccin Mocha theme) with **precision** and **performance**. It is specifically tuned for:

* **Sequence Alignment:** Ligatures are *disabled* to ensure distinct character rendering (e.g., ensuring `=>` or `==` don't merge, which is critical when viewing raw sequence data or code).
* **Large Log Files:** A massive scrollback limit (100k lines) for reviewing extensive pipeline outputs (Nextflow, Snakemake, Bowtie2 logs).
* **Window Management:** Custom keybindings for quick splitting and resizing without touching the mouse.

## 🎨 Features

* **Theme:** Manual implementation of **Catppuccin Mocha** (Dark, high contrast, pastel accents).
* **Font:** **JetBrains Mono** (Size 12).
    * *Note: `calt` and `liga` are disabled for maximum character precision.*
* **Aesthetics:** "Glassmorphism" effect with 95% opacity and 20px blur.
* **Performance:** GPU-accelerated rendering with `xterm-256color` support for rich CLI tools (MultiQC, htop, btop).

## 🛠 Prerequisites

1.  **Ghostty:** [Download here](https://ghostty.org/)
2.  **Font:** [JetBrains Mono](https://www.jetbrains.com/lp/mono/) (Must be installed on your system).

## 📦 Installation

### Option 1: Symlink (Recommended)
Clone this repository and symlink the config file. This allows you to version control your settings easily.

```bash
# 1. Clone the repo
git clone [https://github.com/YOUR_USERNAME/ghostty-bioinformatics-config.git](https://github.com/YOUR_USERNAME/ghostty-bioinformatics-config.git) ~/ghostty-bioinformatics-config

# 2. Backup existing config
mv ~/.config/ghostty/config ~/.config/ghostty/config.backup

# 3. Create Symlink
ln -s ~/ghostty-bioinformatics-config/config ~/.config/ghostty/config

⌨️ Custom Keybindings
This config uses Ctrl + Shift modifiers for window management to avoid conflicts with standard shell commands.

Keybinding
Ctrl + Shift + D	Split Pane Right
Ctrl + Shift + S	Split Pane Down
Ctrl + Shift + T	New Tab	
Ctrl + Shift + Arrows	Navigate Splits
Ctrl + + / Ctrl + -	Zoom Font
Ctrl + 0		Reset Font

🧬 Bioinformatics Optimizations
Scrollback Limit: Set to 100,000 lines.

Why? Essential when running long alignments or builds where you need to scroll up to find the initial error or command.

Clipboard Integration: Read/Write allowed.

Why? Seamless copying of FASTA headers, gene IDs, or error logs directly to/from the system clipboard.

Window Padding: Balanced (8px) for readability without wasting screen real estate.
