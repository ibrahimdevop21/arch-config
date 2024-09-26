# Powerlevel10k Setup Guide for Zsh

This guide will help you install and configure Powerlevel10k, a fast and flexible prompt for Zsh.

## Prerequisites

1. **Zsh**: Ensure you have Zsh installed. You can check by running:
   ```bash
   zsh --version
   ```

2. **Oh My Zsh**: If you haven't already installed Oh My Zsh, follow these steps:
   ```bash
   sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
   ```

## Installation Steps

### Step 1: Install Powerlevel10k

1. Clone the Powerlevel10k repository:
   ```bash
   git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ~/powerlevel10k
   ```

### Step 2: Configure Oh My Zsh to Use Powerlevel10k

1. Open your Zsh configuration file (`~/.zshrc`) in a text editor:
   ```bash
   nano ~/.zshrc
   ```

2. Add or update the following lines:

   ```bash
   # Path to your oh-my-zsh installation
   export ZSH=/usr/share/oh-my-zsh/

   # Set name of the theme to load
   ZSH_THEME="powerlevel10k/powerlevel10k"

   # Path to Powerlevel10k installation
   export POWERLEVEL10K_HOME=~/powerlevel10k

   # Source the Powerlevel10k theme
   source $POWERLEVEL10K_HOME/powerlevel10k.zsh-theme
   ```

### Step 3: Save and Apply Changes

1. Save the changes to `~/.zshrc` and exit the editor (if using nano, press `CTRL + O` to save and `CTRL + X` to exit).

2. Apply the changes by running:
   ```bash
   source ~/.zshrc
   ```

### Step 4: Configure Powerlevel10k

1. The first time you start Zsh after installing Powerlevel10k, it will prompt you to configure the theme. Follow the interactive prompts to customize your prompt as desired.

## Troubleshooting

- If you see a message saying "theme not found," double-check the `ZSH_THEME` and `POWERLEVEL10K_HOME` paths in your `~/.zshrc` file.
- Make sure you have the necessary fonts installed. See the [Powerlevel10k README](https://github.com/romkatv/powerlevel10k#font-installation) for font installation instructions.
