# Install pyenv and python

### 1. [Install python build dependencies](https://github.com/pyenv/pyenv/wiki#suggested-build-environment)

This to update the list of available packages 'apt update' and then install a set of development tools and libraries 'apt install' that are commonly needed for building software from source code:
```
sudo apt update; sudo apt install build-essential libssl-dev zlib1g-dev \
libbz2-dev libreadline-dev libsqlite3-dev curl git \
libncursesw5-dev xz-utils tk-dev libxml2-dev libxmlsec1-dev libffi-dev liblzma-dev
```

### 2. [Install pyenv and additional python versions](https://github.com/pyenv/pyenv-installer)

This command used to download and execute a script directly from the internet using curl and then run it as a shell script with bash.

```
curl https://pyenv.run | bash
```

After that, you will see:

```
WARNING: seems you still have not added 'pyenv' to the load path.

# Load pyenv automatically by appending the following to
# ~/.bash_profile if it exists, otherwise ~/.profile (for login shells)
# and ~/.bashrc (for interactive shells) :

Export PYENV_ROOT="$HOME/.pyenv"
[[ -d $PYENV_ROOT/bin ]] && export PATH="$PYENV_ROOT/bin:$PATH"
eval "$(pyenv init -)"

# Restart your shell for the changes to take effect.

# Load pyenv-virtualenv automatically by adding
the following to ~/.bashrc:
```

Run this command to open bashrc file

```
nano ~/.bashrc
```

Add to bashrc file

```
Export PYENV_ROOT="$HOME/.pyenv"
[[ -d $PYENV_ROOT/bin ]] && export PATH="$PYENV_ROOT/bin:$PATH"
eval "$(pyenv init -)"
```

Reboot or reststart your ubuntu
```
reboot
```

After that install pyenv version 3.10

```
pyenv install 3.10
```

Using pyenv version 3.10 in the environment

```
pyenv global 3.10
```

To check pyenv and python installed, run this command

```
pyenv versions
python --version
```

# [Install NVM](https://github.com/nvm-sh/nvm?tab=readme-ov-file#installing-and-updating)

```
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash
```

Reboot or resstart your ubuntu
```
reboot
```
Then install nvm version 20
```
 nvm install 20
```

# [Install PNPM using corepack](https://pnpm.io/installation)

```
corepack enable pnpm
pnpm
pnpm -v
```
