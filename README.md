# Anypreter - SublimeText2 Plugin

Execute selected Code (or the whole document) from many interpreting laguages directly from your SublimeText2 Editor and see the result

## Installation

You have three ways to install the Anypreter: using git, installing it manually or using the SublimeText2 "Package Controll" (Available here: http://wbond.net/sublime_packages/package_control)

### Install using git

To install this Plugin via git, simply browse to your 'Packages' folder like this:

for Windows

	cd %APPDATA%/Sublime Text 2/Packages

for OS X

	cd ~/Library/Application Support/Sublime Text 2/Packages

for Linux
 
	cd ~/.Sublime Text 2/Packages

for Portable Installations
	
	cd PATH_TO_PORTABLE_INSTALLATION/Sublime Text 2/Data/Packages

and clone this repository

	git clone https://github.com/PhilippSchaffrath/phpInstant


### Install manually

* Download the files using the GitHub .zip download option
* Unzip the files and rename the folder to 'Anypreter' (!IMPORTANT!)
* Copy the folder to your Sublime Text 2 'Packages' directory

### Install using Package Control

If you are familiar with Package Control you definetly know what to do, if not, go to [SublimeText2 - Package Control](http://wbond.net/sublime_packages/package_control) click on 'Install' and follow the instructions

## Settings

The following settings are available and optional, but the default settings should be mostly what you want if you install this plugin
	
	{
		"php_binary_path": "YOUR_PHP_BINARY_PATH",
		"ruby_binary_path": "YOUR_PHP_BINARY_PATH",
		"python_binary_path": "YOUR_PHP_BINARY_PATH",
		"anypreter_stream_output": False,
		"anypreter_output_inteval": 1
	}

php_binary_path: The path to your PHP binary (fallback: "php"-call)
anypreter_stream_output: "True" to buffer the output and display it in a specified interval livetime
anypreter_output_inteval: the output interval for anypreter_stream_output in seconds (can be float)

Streamed output with intervals less then 1 could cause dataloss (its buggy and i dont know why!)

## Usage

To use this plugin, be sure to set your binary paths in your user-settings and use one of this ways to run your interpreter:

* Ctrl+Shift+X To run the first available Mode for this language
* Ctrl+Shift+Y (Quick Panel) and select the Mode you want to run
* Ctrl+Shift+P (Command Palette), type "Anypret" and fire it up
* Rightclick in the document and select "Interpret Code" (only available if the plugin supports this language)

## Release Notes

Anypreter is designed to work with the latest [development build](http://www.sublimetext.com/dev) of Sublime Text 2

## Development

a
If this plugin doesn't supports your interpreting language, please contact me with some information how to run code in your language via the command-line and i will try my best to update it.