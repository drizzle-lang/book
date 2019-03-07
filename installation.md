---
description: Basic Installation Instructions
---

# Installation

## Installing Drizzle

The installation process for Drizzle relies heavily on the presence of Crystal on the host machine. This is due to the fact that Drizzle is an interpreter written in Crystal, and Crystal's static building capabilities are not yet ready. 

{% hint style="warning" %}
Crystal does not yet support Windows and as such, Drizzle can not yet run on Windows
{% endhint %}

### Installing from Source

1. Install Crystal on your computer by following [their guide](https://crystal-lang.org/reference/installation/).
2. Download the archive of the latest release from the [releases page](https://github.com/drizzle-lang/drizzle/releases), unpack it and open a terminal in the directory.
3. Build Drizzle with optimisations using `shards build --release`
4. The built interpreter can be found at `./bin/drizzle`

{% hint style="info" %}
You can also add this binary to your path by running `sudo install bin/drizzle /usr/bin` for system wide or `install bin/drizzle ~/.bin` if you have a bin in your home directory set up. This will allow you to run the `drizzle` command from any directory.
{% endhint %}

## After Installation

Running `drizzle` on its own will open a Read-Eval-Print-Loop \(REPL\) environment for you to mess around in, otherwise passing the command an argument will attempt to open and evaluate a file at the path you specify.

