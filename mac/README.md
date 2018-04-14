# Mac 使用总结

## 安装 [Homebrew](https://brew.sh)
```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```


## 安装 [Homebrew cask](https://caskroom.github.io/)
```
brew tap caskroom/cask
```

之后安装大部分软件只需要用 [Homebrew](https://brew.sh) 和 [Homebrew cask](https://caskroom.github.io/) 即可。

需要破解版的应用的话可以去 [这里找](http://xclient.info/)。


## 推荐软件
```
alfred
atom
bartender
cheatsheet
google-chrome
istat-menus
iterm2
licecap
manico
moon
oh-my-zsh
the-unarchive
```


## brew cask 升级软件
```
brew tap buo/cask-upgrade

brew cu

Usage: brew cu [CASK] [options]
-a, --all             Include apps that auto-update in the upgrade.
--cleanup         Cleans up cached downloads and tracker symlinks after
updating.
-f  --force           Include apps that are marked as latest
(i.e. force-reinstall them).
--no-brew-update  Prevent auto-update of Homebrew, taps, and formulae
before checking outdated apps.
-y, --yes             Update all outdated apps; answer yes to updating packages.
-q, --quiet           Do not show information about installed apps or current options.
```


## QQ登不上清理网络缓存
```
sudo killall -9 networkd
```


## 重置图标
```
defaults write com.apple.dock ResetLaunchPad -bool true; killall Dock
```


## 拷贝 Finder 文件路径
```
Cmd + Opt + C
```


## 显示隐藏文件
```
defaults write com.apple.finder AppleShowAllFiles -bool true ; killall Finder
```


## 隐藏隐藏文件
```
defaults write com.apple.finder AppleShowAllFiles -bool false ; killall Finder
```


## Finder 底部显示路径
```
Cmd + Opt + P
```


## Finder 顶部显示路径
```
defaults write com.apple.finder _FXShowPosixPathInTitle -bool YES
```


## host 文件路径
```
/etc/hosts
```


## 推荐参考

[强迫症的 Mac 设置指南](https://github.com/macdao/ocds-guide-to-setting-up-mac)
[Best App](https://github.com/hzlzh/Best-App)
