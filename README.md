# Vim config

This is my personal vim setup. At present it is only in use for PHP / HTML editing.
There is nothing fancy here.

* Command-T for quick file navigation
* Project settings for per-project config (like indent, expand tab etc)
* Sparkup for making HTML esiting less painful
* Custom 256 colour colour scheme based on http://dengmao.wordpress.com/2007/01/22/vim-color-scheme-wombat/ (requires 256 colour term)
* Pathogen for nice organisation of plugins
* My preferences (ditch the vim-mikesimons bundle if they're not to your liking) 

If you want to give it a try you'll need the following (IIRC):

* git
* python
* ruby
* rake
* rubygems
* libxslt-dev
* bundler (gem)

Once you've got the above:

    git clone git://github.com/mikesimons/vimconfig.git
    cd vimconfig
    git submodule init
    git submodule update
    cd bundle/command-t
    rake make

Now backup your existing vim config and execute the following:

    ln -s <path_to_checkout> ~/.vim
    ln -s ~/.vim/vimrc ~/.vimrc

Obviously if you want to make changes and commit them back to github you'll need to fork.
