# My Confetti Page

Sometimes it takes a long time to run a script, so why not open chrome to this confetti page when your script finishes?

I personally `alias` my confetti command:

```sh
$ my_long_running_command; confetti
```
&nbsp;

I use WSL and can launch Chrome installed on linux with the following command:

```sh
$ google-chrome https://leewarrick.com/confetti --user-data-dir=$(mktemp -d) -incognito --new-window --start-fullscreen --autoplay-policy=no-user-gesture-required > /dev/null 2>&1 &
```
&nbsp;

I also created an alias for Chrome by pointing to the version installed in Windows:

```sh
$ alias google-chrome="/mnt/c/'Program Files (x86)'/Google/Chrome/Application/chrome.exe"
```
&nbsp;

Thanks to the [canvas confetti](https://github.com/catdad/canvas-confetti) library for making this easy!
