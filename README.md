# amazon-music-linux
A standalone app for Amazon Prime Music/Amazon Music Unlimited.

## Installation
[Packages are available in `deb` and `rpm` format](https://github.com/oja/amazon-music-linux/releases).

### Building from source
```
git clone https://github.com/oja/amazon-music-linux
cs amazon-music-linux
npm install
npm run package-linux
```

Then, depending on whether you want to build for Ubuntu/Debian or Fedora/openSUSE, do the following:

- Ubuntu/Debian:
  ```
  sudo npm install -g electron-installer-debian
  electron-installer-debian --src release-builds/amazon-music-linux-linux-x64/ --arch x86_64 --config build-config.json
  ```

- Fedora/openSUSE:
  ```
  sudo npm install -g electron-installer-redhat
  electron-installer-redhat --src release-builds/amazon-music-linux-linux-x64/ --arch x86_64 --config build-config.json
  ```

The output `.deb` or `.rpm` file will be in the `release-builds/` directory.

## TODO
- Media keys support (pause/play, next, last)
- Modify title to playing song

## Legal Disclaimer
No affiliation with Amazon.com, Inc. All trademarks and registered trademarks are the property of their respective owners.
