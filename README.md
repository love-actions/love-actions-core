# love-actions-core

## About

Simple Github Action for packaging `.love` file of a [LÖVE](https://love2d.org/) framework based game.

### Related actions

See related actions below:

[Love actions for android](https://github.com/marketplace/actions/love-actions-for-android)

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
| `build-list`   | `false` | `"./*"`         | List of folder&file paths to be built, separated by spaces |
| `package-path` | `false` | `"./game.love"` | Path to the `.love` package file                         |
