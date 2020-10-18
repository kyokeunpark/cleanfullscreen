# cleanfullscreen
Hides background windows when using fullscreen in BSPWM

This is a fork of [Brodie's script](https://github.com/BrodieRobertson/cleanfullscreen), as it was missing two big feature for me:

1. _Ignore floating windows_ : I use floating terminals which gets hidden/unhidden extremely often (ie., dropdown terminal). This script interferes with dropdown workflow (shows them when I don't want it to). A simple workaround that I have currently is to flat out ignore all floating windows, since I usually do not use floating windows otherwise.
2. _Monocle support_ : BSPWM has an alternative desktop layout called _monocle_. The initial script does not support it, so I just added it myself.

## Usage

Add the following to your bspwmrc:

``` sh
pgrep cleanfullscreen || cleanfullscreen &
```

... and then restart BSPWM (or reload your rc file).
