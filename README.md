# SDR++ Flatpak

This project provides a simple way to install [SDR++](https://github.com/AlexandreRouma/SDRPlusPlus) in non-mutable Operating Systems such as SteamDeck's SteamOS

__WARNING: Tested only with RTL-TCP source on SteamDeck under SteamOS 3.7.x, other usages might need tweaking__

## Building

### Build binaries and dependencies

```
flatpak-builder --force-clean build-dir org.sdrpp.App.yaml --install build-dir --user
```

### Generate single file bundle

```
flatpak build-bundle repo-dir org.sdrpp.App.flatpak org.sdrpp.App
```

Double click `.flatpak` file and install with Discover