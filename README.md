# ionCube PHP extension Toggler for OSX

Inspired by [xdebug-osx][xdebug-osx]

This simple script allows to toggle `on` and `off` [ionCube][ioncube] and is meant for anyone running `PHP` and `ionCube` installed via [Homebrew][brew].


## Installation

```
curl -L https://raw.githubusercontent.com/ytorbyk/ioncube-toggle-osx/master/ioncube-toggle > /usr/local/bin/ioncube-toggle
```

## Installation with clone

```
git clone git@github.com:ytorbyk/ioncube-toggle-osx.git
```

Add `/usr/local/bin` to your `$PATH`. If you use the Bash shell, you can do this by running this command:
```
echo 'export PATH="/usr/local/bin:$PATH"' >> $HOME/.bashrc
```
You may need to restart your shell for this to take effect, or refresh it with `source ~/.bashrc`.

If you want the global command then run:
```
cd ioncube-toggle-osx
ln -s `pwd`/ioncube-toggle /usr/local/bin/ioncube-toggle
```

## Make sure `ioncube-toggle` is executable

```
chmod +x /usr/local/bin/ioncube-toggle
```

## Usage
```
ioncube-toggle                            # outputs the current status
ioncube-toggle on                         # enables ioncube
ioncube-toggle off                        # disables ioncube
ioncube-toggle on|off --no-server-restart # toggles ioncube without restarting apache or php-fpm
```

[brew]: http://brew.sh/
[ioncube]: http://www.ioncube.com
[xdebug-osx]: https://github.com/w00fz/xdebug-osx
