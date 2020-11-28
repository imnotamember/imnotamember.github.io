---
title: Making Pages
layout: "page"
icon: fa-th
order: 6
---

## General workflow:
1. Head to [GitHub](https://github.com) and login to your account.
1. Follow along with the basic set up at [GitHub's documentation for User/Organization Pages development](https://pages.github.com/)
    * Leave your new repository open, as we'll clone it in the near future.
1. Check if you have Ruby installed on your computer by opening a terminal and typing: `ruby -v` 
    1. If you see a version listing of `2.4.0` or greater, then continue. If it's lower than `2.4.0` than you can upgrade it (doubt this will come up, but stop me if so).
    1. If you get an error, than you must install Ruby development environment:
        1. [Windows Installers](https://rubyinstaller.org/downloads/) - Pick the version that has a **bold link** (newest and most compatible)
            * Confirm it worked by running `ruby -v` in GitBash terminal (Press Windows-Key then search for `git-bash.exe`) 
        1. Mac installation:
            * Enter these commands into terminal:
            
            ```BASH
            # First, you need to install the command-line tools to be able to compile native extensions, open a terminal and run:
            xcode-select --install
            
            # Install Homebrew
            /usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
            # Install Ruby via Homebrew
            brew install ruby

            # Add the brew ruby path to your shell config
            export PATH=/usr/local/opt/ruby/bin:$PATH

            # Check to make sure everything installed correctly
            which ruby
            # Should see something like:
            # /usr/local/opt/ruby/bin/ruby

            ruby -v
            # Should see something like:
            # ruby 2.6.2p47 (2019-03-13 revision 67232) [x86_64-darwin18]
            ```
           
        1. Linux (Ubuntu) installation:
            * Enter these commands into terminal:
            
            ```BASH
            echo '# Install Ruby Gems to ~/gems' >> ~/.bashrc
            echo 'export GEM_HOME="$HOME/gems"' >> ~/.bashrc
            echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.bashrc
            source ~/.bashrc
            ```
           
1. Install Jekyll
    1. Windows: in GitBash terminal (Press Windows-Key then search for `git-bash.exe`), 
    1. Mac: in terminal,
    1. Linux: in terminal,
    * Enter the following command: `gem install jekyll bundler`
1. If you're not sure how to clone a repo, check this page out for quick rundown: [GitHub Cloning tutorial](https://help.github.com/en/articles/cloning-a-repository)
1. Clone your website repository from GitHub by issuing the command in you command line: `git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY`
1. You now have a fully functional website repo, now let's dig in!
1. [Setting up a local Jeckyll website](https://help.github.com/en/articles/setting-up-your-github-pages-site-locally-with-jekyll#step-4-build-your-local-jekyll-site)


## Invaluable resources:
1. [GitHub guide to creating GitHub Pages with Jekyll](https://help.github.com/en/articles/using-jekyll-as-a-static-site-generator-with-github-pages)
1. [Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
