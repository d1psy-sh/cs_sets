# README

This is the place for all my notes and the project description.

## CSGO Sets

`cs_sets` is a settings manages for CS:GO in the command line. It should improve saving different configurations adding new configurations and keeping all configurations up to date and backed up.

## Features

- saving configurations in the underlying GitHub Repository
- adding new configurations:
    - new crosshairs
    - new viewmodels
    - new huds
- ... and saving them for later use
- switching configurations on the fly
- downloading pro configurations from configuration sites
- this app is developed on Linux (WSL) and will be compiled for the Windows target structure this is also a test for more cross platform apps in the future

## Infos

In this section I am adding some useful information for developing this app.

- the config.cfg which is the local use configuration that overwrites the default
  configuration is located at `C:\Program Files
  (x86)\Steam\userdata\340818790\730\local\cfg`
- the configuration file is in a structure of <key> <value> where the value can be a float, an integer or a string
- the goal is to parse the config file to a rust `struct` and then modify the
  values, after that we can write the configuration back to the configuration
  file

