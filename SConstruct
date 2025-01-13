#!/usr/bin/env python
import os
import sys

env = Environment()

# Glob search through source files given a specific pattern
sources = Glob("src/*.cpp")

env.Append(CPPPATH=["."])
env.Append(LIBS=["libSumLib"])
env.Append(LIBPATH=["sumlib/lib/"])

env.Append(LINKFLAGS=["-Wl,-rpath," + os.path.abspath("sumlib/lib/")])

# set c++ standard to 11
env.Append(CXXFLAGS=['-std=c++11'])

# Create a runnable program given the source files with all their dependencies
env.Program("helloworld", sources)
