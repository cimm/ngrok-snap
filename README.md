# ngrok snap

UNOFFICIAL. See [ngrok.com](https://ngrok.com/download) for official `ngrok` releases.

This is a first shot at packaging `ngrok` as a [snap](https://www.ubuntu.com/desktop/snappy).

`ngrok` is available via the standard `apt` way on Ubuntu but it's the older version. Since version 2 is no longer open source it can't be added to the official Ubuntu repositories. Bummer. Snaps can help here. I created the `ngrok` snap as a quick way to have the latest and greates `ngrok` version on Ubuntu.

## Installing

If you are running Ubuntu 16.04 LTS or later, you can already use snaps. You only need the `ngrok` snap:

```
sudo snap install ngrok-cimm --beta
```

For other [distros](https://snapcraft.io/docs/core/install) you might want to install `snapd` first.

A snap automatically updates itself as soon as a new version is availble.

## Run

The snap is called `ngrok-cimm`, meaning you'll need to run it with that name as well. You can alway add an alias if that bothers you.

```
$ ngrok-cimm http 5000
```

I could have called it `ngrok` as well but didn't want to squat the `ngrok` name. I'll contact the `ngrok` developer to see if he is interested taking over the package.

## Feedback & bugs

Please report any feedback or bugs as a [GitHub issue](https://github.com/cimm/ngrok-snap/issues).
