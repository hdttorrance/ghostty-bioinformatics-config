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

Keybinding
Ctrl + Shift + D	Split Pane Right
Ctrl + Shift + S	Split Pane Down
Ctrl + Shift + T	New Tab	
Ctrl + Shift + Arrows	Navigate Splits
Ctrl + + / Ctrl + -	Zoom Font
Ctrl + 0		Reset Font
