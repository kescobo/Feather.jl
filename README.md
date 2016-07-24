# Feather

[![0.4](http://pkg.julialang.org/badges/Feather_0.4.svg)](http://pkg.julialang.org/?pkg=Feather)
[![0.5](http://pkg.julialang.org/badges/Feather_0.5.svg)](http://pkg.julialang.org/?pkg=Feather)
[![Travis](https://travis-ci.org/JuliaStats/Feather.jl.svg?branch=master)](https://travis-ci.org/JuliaStats/Feather.jl)
[![Coveralls](https://coveralls.io/repos/github/JuliaStats/Feather.jl/badge.svg?branch=master)](https://coveralls.io/github/JuliaStats/Feather.jl?branch=master)

Package for reading/writing [feather-formatted binary files](https://github.com/wesm/feather) and loading into a Julia DataFrame.

As noted on the official feather homepage, the feather format is still considered "beta" and should not be relied on for
long-term storage/productions needs.

## Installation
```julia
Pkg.add("Feather")
```

## Usage

Feather.jl provides two high-level methods for reading and writing feather files, respectively.
```julia
df = Feather.read("feather_file.feather")

Feather.write("output.feather", df)
```
