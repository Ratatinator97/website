--- 

layout: post
title: "Optimize your Linux experience"
date: 2020-05-01 18:41:35 +0100

---

If you are interested in Gnu+Linux you're in the right place. I started using Linux as my daily drive 2 years ago. At the time I barely knew Linux. Here you'll find my main tools that enable me to have a nice setup and be productive as hell.

## The shell

Is one of the **main tools** if not the main tool of a Linux computer. You will spend a lot of time there and you have to be **comfortable** in there.

Most of the distros are shipped with **Bash**. It's a great and powerful tool but for me it wasn't very enjoyable. Many times my `tab` completion did not work because of a typo. Other times it wasn't handy when selecting items displayed by the `tab` command. Bash's tab auto-completion isn't good enough.

But then I heard of Zsh, a **child** of Bash.

### Zsh

If you had already learned Bash and started to be confident using it then don't worry. Zsh and Bash are very **similar**. Most commands are identical and the logic is the same. Although they seem identical, Zsh have some **improvements** it's father has not ! 

#### Tab Auto-completion

is **great**.

![A picture about the amazing features of Zsh](https://drive.google.com/uc?export=view&id=1NmzyZiOZzeVfV2D72WHs61li2tkaS888)

You can **navigate** through the `tab` results with your `arrow keys` or just pressing `tab` to hop to the next element.

A misspelled `cd documents` will transform into `cd Documents` **magically** !

##### Style

Zsh supports many **theme**s. I don't say Bash hasn't but it's good to know.

##### [Oh my Zsh](https://ohmyz.sh/) !

Is a **great bundle of plugins** and themes ! It is an *incontournable* of Zsh.

I won't go through the plugins as they are already documented in their website.

###### Be Carefull: you have to use the `.zshrc` instead of the `.bashrc` .

## Battery optimization

A lot of students and developers out there use **laptops** as main computers when it comes to **work**. Most of our devices doesn't last a day. I see a lot of colleagues that are plugged in more than <u>two times a day</u> and they make me suffer because Linux has a **lot** of battery optimization tools.

#### TLP

I don't know what TLP stands for but I know it gives me more than **2h** of **battery** ! The install and setup is straightforward. Satisfaction guaranteed !

Here is the link to the [documentation]([TLP - Optimize Linux Laptop Battery Life &mdash; TLP 1.3.1 documentation](https://linrunner.de/tlp/index.html)) !

#### Powertop

It is another one battery optimizer. It gives me the same results that with TLP.

## Zram, Zswap or Zcache ?

Linux offers many solutions when it comes to optimize. You have seen two battery optimization tools. But what about **Ram** optimization ?

When you define partitions for your Linux OS, you are often offered a Swap partition. Swap is a "fake" Ram, it acts like it but as it is stored in your hard drive it is **much slower** than your Ram (physical). Yet not, don't delete that partitions because Swap is very useful.

So here we face multiple positions :

- If you **don't** have a Swap partition then go for Zram

- If you have Swap go for Zswap

- If you like risks and want bleeding edge tools go for Zcache, is it not ready yet but it does a better job than Zswap.
  
  If you want to know more about it, I recommend you to read [this post]([kernel - zram vs zswap vs zcache Ultimate guide: when to use which one - Ask Ubuntu](https://askubuntu.com/questions/471912/zram-vs-zswap-vs-zcache-ultimate-guide-when-to-use-which-one)) on StackExchange.

## Gnome

For the Ubuntu or the elementary OS you may know your DE (desktop env.) is   GNOME. I personally use Gnome under Wayland and I find it very good. It is the main alternative of Kde at this time and same you're not fan of WM's (Window Managers).

### Gnome vanilla is nice but can be improved

If you don't use Ubuntu then you may want to use [Snapcraft](https://snapcraft.io/) as well. It is a widely popular "App" Store. It is developed by Canonical so only Ubuntu based distributions support it in native. **But other distros can use it too !**

If you build your Linux from scratch you may want to have **Flatpack** too. It is installed on Gnome by default.

One thing that is very important is to be careful of the **permissions** of the snap/flatpack package. They are usually **very restricted** (i.e. can only use the `~/` by default). If you have a package that needs access to `/bin` or `/usr` you have to **give** then the access to it. You can learn more about it [there]([Sandbox Permissions &mdash; Flatpak documentation](https://docs.flatpak.org/en/latest/sandbox-permissions.html)).

### [ UnixPorn]([r/unixporn - the home for *NIX customization!](https://www.reddit.com/r/unixporn/))

Gnome isn't as flexible as Wm's or Kde when it comes to style. But it can **change** a lot and improve. 

> One of the mains reasons to choose Linux over Windows or Mac is that you can and you may tailor your OS for your personal needs. You don't use a "for everyone" OS. You have your own OS that is optimized for your workflow.

For that you have to install `gnome-tweak-tools`. This module enables you to install extensions from [GNOME Shell Extensions](https://extensions.gnome.org/#). It can be added with **ease** from this website. If you want to change the style then. You'll find **extensions** such as Caffeine, Dash to Dock, User Themes etc. 

I recommend you use [Gnome Shell Themes - Gnome-look.org](https://www.gnome-look.org/browse/cat/134/order/latest/) as **theme** store for Gnome. The themes are easily installable as you have a superb [helper](https://www.pling.com/p/1136805/).


