# Gemi-cli

## Description: It is a simple CLI tool built to use Google's Gemini from the command line. 

## Features:
- Gemini is multi-modal so it can read images and texts and answer questions on them based on the prompt given
- It can also be used to have a multi-turn conversation with Gemini

## Examples
```
usage: gemi-cli [-h] [-c] [-ri image_location] [-rt file_location] [-p prompt]

gemi-cli - A CLI application to access gemini from your command line. :)

options:
  -h, --help            show this help message and exit
  -c, --chat            Start a conversation with gemini
  -ri image_location, --read-image image_location
                        Show image at specified location.
  -rt file_location, --read-file file_location
                        Read contents of the specified file.
  -p prompt, --prompt prompt
                        Add a prompt for the image
```

### Reading an image
![image](https://github.com/slayeh17/gemi-cli/assets/104914725/15cfc387-286e-4520-b2fd-6b4767c0b7a9)

### Reading a C code file
![image](https://github.com/slayeh17/gemi-cli/assets/104914725/2fb4002e-ba64-4f36-8d42-18a57b141e8d)

### Conversation 
![image](https://github.com/slayeh17/gemi-cli/assets/104914725/c32df4a6-59ae-4e38-a241-8bf4e215f32b)


## Installation 
- Clone the repo
- Run `pip install -r requirements.txt`
- Execute `chmod +x gemi-cli`
- Execute `pwd` which should give you your current location
- If you are using `zsh` then add this line to your `.zshrc` file `export export PATH=$PATH:"the path got from pwd"`. If you are using `bash` add the `export` line to your `.bashrc` file
- Execute `source ~/.zshrc` or `source ~/.bashrc`
- Now you can use the `gemi-cli` command from anywhere in your machine

## Uninstallation
- Remove the `export` line from `.zshrc` or `.bashrc`
- Run `pip uninstall -y -r requirements.txt`
- Now you have remove `gemi-cli` from your machine