# My Confetti Page

Sometimes it takes a long time to run a script, so why not open chrome to this confetti page when your script finishes?

I personally `alias` my confetti command:

```sh
$ my_long_running_command; confetti
```
&nbsp;

I use WSL and can launch Chrome installed on linux with the following command:

```sh
$ google-chrome https://leewarrick.com/confetti --new-window --start-fullscreen --autoplay-policy=no-user-gesture-required > /dev/null 2>&1 &
```
&nbsp;

Here's how I installed Chrome on Linux with WSL:

```sh
$ sudo apt update && sudo apt -y upgrade && sudo apt -y autoremove
$ wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
$ sudo apt -y install ./google-chrome-stable_current_amd64.deb
```
&nbsp;

Thanks to the [canvas confetti](https://github.com/catdad/canvas-confetti) library for making this easy!
