# Flutter latest docker action

To create actions using `flutter` command you can use this action

## Inputs
no inputs

## Outputs
test

## Example usage

```
jobs:
  build:
    name: run testing
    runs-on: ubuntu-latest
    steps:
    - uses: actions/checkout@v1

    - name: install dependencies
      uses: geowatson/flutter-latest@1.0.0
      with:
        args: pub get

    - name: run tests
      uses: geowatson/flutter-latest@1.0.0
      with:
        args: test
```
