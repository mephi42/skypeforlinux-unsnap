# skypeforlinux-unsnap

Run skypeforlinux without snap.

## Scripts

### `./00-download`

Downloads the latest stable amd64 skypeforlinux into `./skype.snap`.

### `./01-extract`

Extracts the contents of `./skype.snap` into `./fs`.

### `./02-run`

Starts skypeforlinux from `./fs`.

### `./03-desktop`

Creates a `skypeforlinux-unsnap.desktop` file for `./02-run`.

## Troubleshooting

Tested on amd64 Ubuntu 24.04, YMMV.

For a different distro, `LD_LIBRARY_PATH` or `patchelf` might be necessary.

If the Skype icon appears in the tray, but the Skype window doesn't open, try
deleting `~/.config/skypeforlinux`.
