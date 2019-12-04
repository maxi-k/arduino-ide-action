# GitHub Action to install Arduino IDE

## Usage

### Example Workflow file

```yaml
jobs:
  build:
    runs-on: ubuntu-latest
    steps:
    - uses: actions/checkout@master
    - name: Install Arduino IDE
      uses: me-no-dev/arduino-ide-action@master
        with:
          ide_path: arduino-ide # optional: relative to $HOME or absolute. default: $HOME/arduino-ide
          usr_path: Arduino # optional: relative to $HOME or absolute. default: $HOME/Arduino
          ide_version: nightly # optional: version of the arduino IDE to download. default: nightly 

...
    - run: |
        ...
```

## License

The Dockerfile and associated scripts and documentation in this project are released under the [MIT License](LICENSE).
