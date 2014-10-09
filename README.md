h3rbz_custom Color Theme for irssi
==================================

Initially created by [h3rbz](http://irssi.org/themes), this is a
theme for the [irssi](http://irssi.org/) IRC chat client with my personal
modifications to the original [h3rbz irssi theme](http://irssi.org/themefiles/h3rbz.theme)
and if others enjoy it, then all the better.

I use this with the Solarized theme with gnome-terminal and KDE’s konsole.

[irssi](http://www.irssi.org/)

[Solarized](http://ethanschoonover.com/solarized)

[Solarized Gnome-terminal](https://github.com/Anthony25/gnome-terminal-colors-solarized)

Note: This will be [default](http://fedoramagazine.org/fedora-21-will-feature-solarized-color-schemes-in-both-the-terminal-and-gedit/) in Fedora 21 GNOME

Solarized has been available by default in KDE for years.

Visit the Solarized homepage
----------------------------

See the [Solarized] homepage for screenshots, details and color theme
implementations for terminal emulators and other applications, such as Vim,
Emacs, and Mutt.

Installation
------------

1.  Obtain `solarized-universal.theme`

    a) Option A: Download `h3rbz_custom.theme` from here
       and place it in your `~/.irssi` directory

    b) Option B: To always have the latest version, clone the git repository:

        $ git clone https://github.com/maxamillion/irssi-h3rbz-custom.git
        $ ln -s $PWD/irssi-h3rbz-custom/h3rbz_custom.theme ~/.irssi/

2.  Change your `~/.irssi/config` to include the following settings, while making
    sure to replace `YOUR_NICKNAME` with your IRC nickname:

        settings = {
            ...
            "fe-common/core" = {
                ...
                theme = "h3rbz_custom";
                hilight_color = "= %R";
            };
            ...
        };
        hilights = (
                { text = "YOUR_NICKNAME"; color = "%M"; nick = "yes"; word = "yes"; }
        );

