# NEW MAC SETUP 2023

## Install iTerm and Homebrew
- [Install iTerm](https://iterm2.com/)
- [Install Homebrew](https://brew.sh/)

## Install Fira Code Font

See [Fira Code installation docs](https://github.com/tonsky/FiraCode/wiki/VS-Code-Instructions)
```bash
brew tap homebrew/cask-fonts
brew install --cask font-fira-code
```

## Set up iTerm, Zsh, and plugins

Zsh is the default shell for Mac.

- Install iTerm their docs
- [Configure Terminal with Oh My Zsh!](https://engineeringfordatascience.com/posts/configure_terminal_for_data_science_with_oh_my_zsh/)

## Generate SSH Key

See more details on [Github docs](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)

```bash
ssh-keygen -t ed25519 -C "your_email@example.com"
```
Add it to Github and remove keys from older machines from [Github UI](https://github.com/settings/keys).

### Install NVM and Node.js

See [here](https://github.com/nvm-sh/nvm) for the latest guide

```bash
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.3/install.sh | bash

# This will install the latest node version
nvm install node
```

## Install Visual Studio Code

Install the editor from their website. And then add the shortcut to `.zprofile` so that you can open a workspace with `code /path/to/the/workspace`.

```bash
cat << EOF >> ~/.zprofile
# Add Visual Studio Code (code)
export PATH="\$PATH:/Applications/Visual Studio Code.app/Contents/Resources/app/bin"
EOF
```

> Login with Github, and sync everything. This will bring all the settings and the extensions.

## Install Java

```bash
brew install java
echo 'export PATH="/usr/local/opt/openjdk/bin:$PATH"' >> ~/.zshrc
```
