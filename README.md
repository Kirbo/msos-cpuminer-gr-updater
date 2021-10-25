# msOS cpuminer-gr updater

One command to install/update the cpuminer-gr on [msOS](https://minerstat.com/software/mining-os).

## Prerequisites

Make sure you have CPU mining enabled and using `cpuminer-opt` client in minerstat worker configs.
See the [minerstat CPU mining guide](https://minerstat.com/help/cpu-mining).

You'll find the `cpuminer-gr` versions [here](https://github.com/WyvernTKC/cpuminer-gr-avx2/releases).
And the executable variatons [here](https://github.com/WyvernTKC/cpuminer-gr-avx2/blob/main/readme.txt#L88).

## Installation

```shell
git clone https://github.com/kirbo/msos-cpuminer-gr-updater.git ~/msos-cpuminer-gr-updater
echo 'export PATH="~/msos-cpuminer-gr-updater/commands:$PATH"' >> ~/.bashrc
source ~/.bashrc
```

## How to update this repository

If there are any updates on these commands, just run the following command to update:

```shell
kirbo-msos-repository-updater
```

## How to install/update cpuminer-gr

You just need to run this command

```shell
cpuminer-updater <version> <executable variation>
```

For example on my machine, I have `AMD Ryzen 5 3600 6-Core Processor` and `AMD Ryzen 7 3700X 8-Core Processor`,
so I need to use the `cpuminer-zen2` executable.
In my case, if I wanted to install `cpuminer-gr` version `1.2.3` for my Ryzens, I should run command:

```shell
cpuminer-updater 1.2.3 zen2
```
