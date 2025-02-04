# File Structure Builder

A Python-based tool that allows users to generate and manage file structures from a structured definition file. It can be used via a command-line interface (CLI) to automate project scaffolding.

## Features
- Build directory structures from a text definition.
- Parse structured files to generate folder hierarchies.
- CLI interface for ease of use.
- Supports interactive mode (future implementation).

# File Structure Builder - User Guide

## Installation
To install `file-structure-builder`, run:
```sh
pip install file-structure-builder
```
After installation, you can use the `fsb` command in your terminal.

## Usage

### 1. Create a File Structure from a Text File
Prepare a text file (e.g., `structure.txt`) with your desired file structure:
```
project-root/
    ├── src/
    │   ├── main.py
    │   ├── utils.py
    │   ├── config/
    │   │   ├── settings.json
    │   │   ├── database.json
    ├── tests/
    │   ├── test_main.py
    ├── README.md
```
Then, run:
```sh
fsb --file structure.txt
```
This will create the directory structure as defined in `structure.txt`.

### 2. Interactive Mode
You can start an interactive session where you describe your structure:
```sh
fsb --interactive
```
It will prompt you to enter the desired file structure.

### 3. Fetch Structure from API (Future Feature)
(Not implemented yet)
```sh
fsb --api
```

## Command-Line Options

| Command | Description |
|---------|------------|
| `fsb --file <file.txt>` | Creates file structure from a text file |
| `fsb --interactive` | Opens an interactive session to define structure |
| `fsb --api` | (Future) Fetch structure from API |

## Example Usage

### Example 1: Creating a Basic Project Structure
```sh
fsb --file my_structure.txt
```
This will read `my_structure.txt` and create directories and files.

### Example 2: Interactive Mode
```sh
fsb --interactive
```
Follow the instructions to build a structure manually.

## Uninstalling
To remove `file-structure-builder`:
```sh
pip uninstall file-structure-builder
```


## Module Overview
### `file_structure_builder/builder.py`
Handles creating directories and files based on a structured input list.

### `file_structure_builder/parser.py`
Parses text-based structure files and converts them into a structured format for processing.

### `file_structure_builder/utils.py`
Placeholder for utility functions (future expansion).

## Roadmap
- [ ] Implement API-based structure fetching.
- [ ] Add interactive mode.
- [ ] Improve error handling and logging.

## Contributions
Contributions are welcome! Feel free to submit issues and pull requests.

## Author
[Aliasghar Mirshahi](https://github.com/aliasgharmirhshai/)

