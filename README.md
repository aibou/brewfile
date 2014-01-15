# Brewfile

## Usage

    # install XCode
    # install XCode Command Line Tools
    ruby -e "$(curl -fsSL https://raw.github.com/Homebrew/homebrew/go/install)"
    sudo gem install brewdler
    # edit cask-installer.rb
    sudo vi /Library/Ruby/Gems/1.8/gems/brewdler-0.5.0/lib/brewdler/cask_installer.rb
      > if system 'brew cask info'
      < if system 'brew cask > /dev/null'
    
    brewdle install