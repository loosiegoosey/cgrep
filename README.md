# cgrep

## Overview
`cgrep` is a Contextual Grep tool designed to search file(s) for a matching string and display the surrounding chunks of text. This utility enables quicker searching through files without needing to open them in an editor to perform find operations.

## Features
- Search for specific text patterns within files.
- Display surrounding context lines around the matched string.
- Easily integrates with command-line workflows.

## Installation Instructions

1. **Clone the Repository**
    ```bash
    git clone https://github.com/Yuriy/cgrep.git
    cd cgrep
    ```

2. **Install Dependencies (if any)**
    While the current code does not specify any external dependencies, it's always a good practice to ensure you have a suitable Python environment. You can set this up with the following:
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. **Run the Script**
    You can directly run the script using Python:
    ```bash
    python cgrep.py [options]
    ```

## Usage Examples
Here’s how you can use the `cgrep` tool from the command line:

```bash
python cgrep.py -n 5 -p 'search_pattern' filename.txt
```
- `-n` : Number of context lines to display around the matched text.
- `-p` : The pattern or string to search for in the file.
- `filename.txt` : The file where the search needs to be performed.

## Code Summary
The project currently consists of a single file, `cgrep.py`, which implements the main functionality of the `cgrep` tool.

### Key Files
- **cgrep.py**:
    - **ContextualGrep Class**: 
        - `__init__(self, numlines)`: Initializes the `numlines` parameter to control the number of lines to be displayed around the matching string.
        - `grep(self, pattern, file)`: Proposed method (though incomplete in the content provided) to search for the specified pattern in the given file and display context lines.

## Contributing Guidelines
We welcome contributions from the community. Here’s how you can help:

1. **Fork the Repository**
2. **Create a Feature Branch**
    ```bash
    git checkout -b feature_branch
    ```
3. **Commit your Changes**
    ```bash
    git commit -m 'Add some feature'
    ```
4. **Push to the Branch**
    ```bash
    git push origin feature_branch
    ```
5. **Create a Pull Request**

Please ensure your code adheres to the existing coding conventions and passes all tests.

## License
This project is licensed under the terms of the MIT License. See the [LICENSE](LICENSE) file for details. 

---

Disclaimer: Portions of the original code appear incomplete or indicative placeholders; further refinements might be required based on the complete logic and additional files within the project repository.