# means-of-production
reusable workflows for my repos

# python setup
```
# install homebrew, this lets you install many other programs using 'brew install'
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

# install pyenv, a python version manager
brew update
brew install pyenv
brew install pyenv-virtualenv

# edit your ~/.zshrc to look like this
export PYENV_ROOT="$HOME/.pyenv"
export PATH="$PYENV_ROOT/bin:$PATH"
eval "$(pyenv init --path)"

if command -v pyenv 1>/dev/null 2>&1; then
    eval "$(pyenv init -)"
    eval "$(pyenv virtualenv-init -)"
fi
export PYENV_VIRTUALENV_DISABLE_PROMPT=1

# install whichever global python version you want
pyenv install 3.11.4
pyenv global 3.11.4

# verify that it the same version
python --version

# install poetry
brew install poetry
```