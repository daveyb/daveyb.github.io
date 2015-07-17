---
layout: post
title: Gotchas with knife-azure gem on Yosemite
---

I ran into some issues with the [chef/knife-azure](https://github.com/chef/knife-azure) installation and configuration sections of the README, so I'm writing them down here.

##Installation##

`sudo gem install knife-azure` fails. I found a good writeup on this here: http://effectif.com/ruby/installing-nokogiri-on-mavericks

I'm using rvm, not rbenv, but the solution that worked for me is pretty much the same:

1. `xcode-select --install`
2. `sudo gem install nokogiri` which, in my case, was the knife-azure dependency that was causing the build error.
3. `sudo gem install knife-azure`

Once the gem installs, it should be available in your shell $PATH. Try running `knife azure --help` to confirm.

##Configuration##

Once you've downloaded your Azure publishsettings file (https://manage.windowsazure.com/publishsettings/index?client=xplat), you have to tell knife where to find that file so it can communicate with your Azure account. The publishsettings file is actually a really convenient way to authenticate to Azure.

*DO NOT check your publishsettings file into GitHub*, for obvious reasons.

You'll find your knife.rb file in ~/chef-repo/.chef or ~/.chef. If it isn't there, create it manually or run `knife configure`.

Simple.

Add to your knife.rb file

`knife[:azure_publish_settings_file] = "/full/path/to/myazure.publishsettings"`

- Don't use a relative path or your home path "~/" as indicated in the README. If you do, you'll get an error

```
WARNING: no knife configuration file found
```

![](https://raw.githubusercontent.com/daveyb/daveyb.github.io/master/images/knife-azure-error.png)

After configuring knife.rb correctly, you should be able to get started using knife-azure!
