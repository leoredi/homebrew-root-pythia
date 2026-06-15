# Homebrew ROOT with optional PYTHIA 8

This tap packages CERN ROOT with an optional `TPythia8` integration.
The default build matches Homebrew's ROOT feature selection and leaves
PYTHIA disabled.

## Install

Build ROOT without PYTHIA:

```sh
brew install leoredi/root-pythia/root
```

Build ROOT with PYTHIA 8 and `TPythia8`:

```sh
brew install leoredi/root-pythia/root --with-pythia
```

Verify the optional integration:

```sh
root-config --has-pythia8
```

The expected output for the optional build is `yes`.
