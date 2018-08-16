# dlmagnet

Start a torrent from a magnet link by calling an API.

Feel free to open an issue / submit a PR, I'm really open to any suggestions!

## Installing

This is a very manual installation.

1. copy `dlmagnet` to `/usr/local/bin/` and make it executable

```sh
42sh# cp dlmagnet /usr/local/bin
42sh# chmod +x /usr/local/bin/dlmagnet
```

2. edit the `/usr/local/bin/dlmagnet` script to specify a command that fits your
needs for downloading a torrent (the magnet link is provided as first and only
argument to `dlmagnet`, between simple quotes).

3. copy `dlmagnet.desktop` to your local application folder

```sh
42sh$ cp dlmagnet.desktop ~/.local/share/applications
```

4. set `dlmagnet.desktop` as the default app when handling magnet uri

```sh
42sh$ xdg-settings set default-url-scheme-handler magnet dlmagnet.desktop
```

## License

[MIT](./LICENSE)
