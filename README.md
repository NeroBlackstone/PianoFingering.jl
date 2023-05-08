# PianoFingering.jl

PianoFingering.jl is an automatic fingering generator for piano scores, written in the Julia language.

![image](./example.png)

THIS PACKAGE ONLY TESTED ON LINUX.

## How to use it

### Pre-requirement

> Prompt: You can copy all following commands start with ❯ 

Install Python (>3.11) and Julia (>1.8). 

Make sure:

``` shell
❯ python -V
Python 3.11.3
❯ julia -v
julia version 1.8.5
```

Install `music21`:

``` shell
❯ pip3 install music21
```

Clone this project to your computer and change directory to `PianoFingering.jl` folder, then:

``` shell
❯ julia
❯ using Pkg
❯ Pkg.activate(".")
❯ Pkg.instantiate()
```

Now you have installed all the dependency. Close your terminal.

### Run Programe

1. Put your `.musicxml` file to `musicxml` folder, suppose we have an `example.musicxml` file right now.

2. Change directory to `PianoFingering.jl` folder:

``` shell
❯ julia -t auto
❯ using Pkg
❯ Pkg.activate(".")
❯ using PianoFingering
❯ fingering("example")
```

Wait for the program to complete, annotated piano score `example_output.musicxml` will be stored in `output` folder, this may take a few minutes.

### Feedback

If you encounter error, or musicxml file can't fingering correctly. Please open a issue and upload your musicxml file.
