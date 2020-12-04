# ngrok snap

[![Get it from the Snap Store](https://snapcraft.io/static/images/badges/en/snap-store-white.svg)](https://snapcraft.io/ngrok-cimm)

UNOFFICIAL. See [ngrok.com](https://ngrok.com/download) for official `ngrok` releases.

`ngrok` is available via the standard `apt` way on Ubuntu but it's the older version. Since version 2 is no longer open source it can't be added to the official Ubuntu repositories. Bummer. Snaps can help here. I created the `ngrok` snap as a quick way to have the latest and greatest `ngrok` version on Linux.

## Installing

If you are running Ubuntu 16.04 LTS or later, you can already use snaps. You only need the `ngrok` snap:

```
$ snap install ngrok-cimm
```

For other [distros](https://snapcraft.io/docs/core/install), you might want to install `snapd` first.

A snap automatically updates itself as soon as a new version is available.

## Run

The snap is called `ngrok-cimm`, meaning you'll need to run it with that name as well. You can always add an alias if that bothers you.

```
$ ngrok-cimm http 5000
```

I could have called it `ngrok` as well but didn't want to squat the `ngrok` name. I'll leave that to for the official `ngrok` snap.

## Building

You can build the snap yourself if you are a developer via [Snapcraft](https://snapcraft.io/). Clone this repo and run `snapcraft` from the root directory:

```
$ git clone https://github.com/cimm/ngrok-snap.git
$ cd ngrok-snap
$ snapcraft
```

You can now install the snap locally (add `--devmode` since the snap you built has not been signed by the store).

```
$ sudo snap install ngrok-cimm*.snap --devmode
```

## Feedback & bugs

Please report any feedback or bugs as a [GitHub issue](https://github.com/cimm/ngrok-snap/issues).

## Disclaimer & license

I am not affiliated in any way with the official [ngrok](https://ngrok.com/download) project. This git repo is licensed under the MIT license but I have no say over the proprietary ngrok binary.
