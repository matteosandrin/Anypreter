# Anypreter - Sublime Text 3 Plugin

Execute selected Code (or the whole document) from many interpreting laguages directly from your Sublime Text 3 Editor and see the result.

This packaged is equal in functionality to the one build by [phisch](https://github.com/phisch/Anypreter), but updated to work with Sublime Text 3 and Python 3.

### Supported Interpreters

* Python 2
* Python 3
* Ruby

## Installation

* Download the files using the GitHub .zip download option
* Unzip the files and rename the folder to 'Anypreter'
* Copy the folder to your Sublime Text 3 'Packages' directory

## Settings

The following settings are available and optional, but the default settings should be mostly what you want if you install this plugin

```json
	{
		"ruby_binary_path": "/path/to/ruby",
		"python_binary_path": "/path/to/python",
		"anypreter_stream_output": false,
		"anypreter_output_inteval": 1
	}
```

* `ruby_binary_path`: The path to your python binary
* `python_binary_path`: The path to your python binary
* `anypreter_stream_output`: `true` to buffer the output and display it in a specified interval livetime
* `anypreter_output_inteval`: the output interval for `anypreter_stream_output` in seconds (can be float)

## Usage

To use this plugin, be sure to set your binary paths in your user-settings and use one of this ways to run your interpreter:

* `Ctrl+Shift+X` To run the first available Mode for this language
* `Ctrl+Shift+Y` (Quick Panel) and select the Mode you want to run
* Right click in the document and select "Interpret Code" (only works if language is supported)