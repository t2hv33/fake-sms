## Fake-SMS
Fake-SMS is a simple command line tool written in Go that allows you to bypass phone number based SMS verification by using a temporary phone number as a proxy. It provides an interactive CLI for easy use and includes a local file-based database to save and manage a list of fake phone numbers for future use.

The latest update for Fake-SMS replaces the previous phone number provider with a new one that offers more phone numbers across more countries. Make sure to pull the main branch before compiling to ensure you have the latest version.

### Features:
- Written in Go-1.15 with modules support enabled
- Interactive CLI for easy usage
- Local file-based database for storing and managing fake phone numbers

### Requirements:
- Go programming language - version 1.15 or higher

### Build Instructions:
To build Fake-SMS, follow these simple steps:

1. Set the `GOBIN` environment variable to the current working directory:
```
export GOBIN=$PWD/bin
```
2. Install the tool:
```
go install
```
This will build the binary and place it in the `bin/` directory. Alternatively, you can download the pre-built binary from the `bin/` directory.

### Usage Steps:
1. Register a number in the local database:
You can register a number by selecting one of the available numbers. This step is demonstrated in the following gif:

![register-number](./gifs/add.gif)

2. Get the messages from a registered number:
You can select a number that was saved in the previous step and view its messages as a list. The tool will also save the message dump as a JSON file in the format `${PWD}/selected-phone-number.json`. This step is demonstrated in the following gif:

![get-messages](./gifs/messages.gif)

3. Optionally, you can choose to delete the remembered numbers or list them.

#### Acknowledgements
There is a similar tool available in pure shell script. You can check it out [here](https://github.com/sdushantha/tmpsms).

#### Contributing
While the tool is simple, any suggestions, enhancements, or bug fixes from the community are welcomed. Please open an issue to discuss or make a pull request directly!
