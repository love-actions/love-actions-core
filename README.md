# love-actions-core

## About

Simple Github Action for packaging `.love` file of a [LÖVE](https://love2d.org/) framework based game.

### Related actions

See related actions below:

[Love actions for testing](https://github.com/marketplace/actions/love-actions-for-testing)

[Love actions for android](https://github.com/marketplace/actions/love-actions-for-android)

[Love actions for iOS](https://github.com/marketplace/actions/love-actions-for-ios)

[Love actions for Linux](https://github.com/marketplace/actions/love-actions-for-linux)

[Love actions for macOS portable](https://github.com/marketplace/actions/love-actions-for-macos-portable)

[Love actions for macOS App Store](https://github.com/marketplace/actions/love-actions-for-macos-app-store)

[Love actions for Windows](https://github.com/marketplace/actions/love-actions-for-windows)

## Quick example

```yaml
- name: Build bare love package
  uses: 26F-Studio/love-actions-core@main
  with:
    build-list: ./assets/ ./frameworks/ ./config.lua ./main.lua
    package-path: ./bare/my_game.love
```

## All inputs

| Name             | Required  | Default           | Description                                                |
| :--------------- | --------- | ----------------- | ---------------------------------------------------------- |
| `build-list`     | `false`   | `"./*"`           | List of folder & file paths to be built. Separated by spaces |
| `package-path`   | `false`   | `"./game.love"`   | Path to the `.love` package file                           |
