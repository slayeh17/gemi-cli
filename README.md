# Gemi-cli

## Description: It is a simple CLI tool built to use Google's Gemini from the command line. 

## Features:
- gemi cli can read a text file and answer questions based on the prompt
- It can read an image and answer questions based on the prompt
- It can read small pdfs (4-8 pages) and answer questions based on the prompt
- It can read a single page of a pdf and answer questions based on the prompt

## YouTube Demo [Link](https://www.youtube.com/watch?v=vsF067nVfek)

## Examples
```
usage: gemi-cli [-h] [-c] [-ri image_location] [-rf file_location] [-rpdf file_location]
                [-page page_number] [-p prompt]

gemi-cli - A CLI application to access gemini from your command line. :)

options:
  -h, --help            show this help message and exit
  -c, --chat            Start a conversation with gemini
  -ri image_location, --read-image image_location
                        Show image at specified location.
  -rf file_location, --read-file file_location
                        Read contents of the specified file or small pdfs.
  -rpdf file_location, --read-pdf-file file_location
                        Read contents of a specified page from a pdf file.
  -page page_number     Specify page number for PDF file.
  -p prompt, --prompt prompt
                        Add a prompt
```

### Reading an image
![image](https://github.com/slayeh17/gemi-cli/assets/104914725/15cfc387-286e-4520-b2fd-6b4767c0b7a9)

### Reading a C code file
![image](https://github.com/slayeh17/gemi-cli/assets/104914725/2fb4002e-ba64-4f36-8d42-18a57b141e8d)

### Conversation 
![image](https://github.com/slayeh17/gemi-cli/assets/104914725/c32df4a6-59ae-4e38-a241-8bf4e215f32b)


## Installation 
- Clone the repo and `cd` into it
- Run `pip install -r requirements.txt`
- Execute `chmod +x gemi-cli`
- Execute `pwd` which should give you your current location
- If you are using `zsh` then add this line `export PATH=$PATH:"the path got from pwd"` to your `.zshrc` file. If you are using `bash` add the `export` line to your `.bashrc` file
- Execute `source ~/.zshrc` or `source ~/.bashrc`
- Now you can use the `gemi-cli` command from anywhere in your machine
- At first you'll be asked to get the API_KEY. After getting the API_KEY rename the `.env_example` file to `.env` and paste the Key there

## Uninstallation
- Remove the `export` line from `.zshrc` or `.bashrc`
- Run `pip uninstall -y -r requirements.txt`
- Now you have removed `gemi-cli` from your machine
