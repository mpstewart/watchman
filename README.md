# watchman

`watchman` uses filesystem watching tools to run commands

## Dependencies

- `carton`, to manage the Perl dependencies

## Installation

1. Clone the repo
2. `cd` into the repo
3. Run `carton install`
4. Add `watchman/bin` to your `$PATH`

## Usage

```
watchman -- make test
```

`watchman` will look for Perl file changes in the current directory, and when a file is written, it will run your command.

## Limitations

Right now, `watchman` only watches for changes in Perl files. So, files with a `.pl`, `.pm`, or `.t` extension. I will probably add support for other languages at some point, but I don't need it right now.
