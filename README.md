# TidalCycles plugin for Atom

[TidalCycles](https://tidalcycles.org) is a live-coding pattern language

For installation instructions, please visit:
  http://tidalcycles.org/getting_started.html

Then, you can:
  * Open a `.tidal` file

  * `shift+enter` to evaluate the current line or selection

  * `cmd+enter` to evaluate multiple-lines or selection

To send patterns to [SuperDirt](https://github.com/musikinformatik/SuperDirt), use `d1` .. `d9`, e.g.:

````
d1 $ sound "bd cp"
````

To send patterns to [classic dirt](https://github.com/tidalcycles/dirt), use `c1` .. `c9`, e.g.:

````
c1 $ sound "bd cp"
````

# Configurable Boot Options

By default, Atom will use a default Tidal bootup sequence that doesn't really do
anything special other than create the `d1..d9` and `c1..c9` Dirt connections.

If you'd like to provide a path to your own custom boot file on your computer, use
the *Boot Tidal Path* setting to do so.

Further, if you'd like Atom to locate a `BootTidal.hs` file in the current directory,
check the *Use Boot File In Current Directory* option.

Boot file order of precedence:

1. Current directory `BootTidal.hs`
2. Custom Boot Tidal Path
3. Default bootup provided by the package

# Contributing

If you'd like to contribute to this package, here are some guidelines:

## JavaScript Formatting

A `.jsbeautifyfc` file is used to define JavaScript formatting settings. Please use
a beautifier package (we recommend `atom-beautify`) to format your changes with
these settings.
