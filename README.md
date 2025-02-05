# dtree - Directory Tree Visualizer

A lightweight command-line tool that generates a clear, visual representation of directory structures. Perfect for documentation, project overview, or understanding complex folder hierarchies.

### Requires Python3 to be installed

## Features

- 🌲 Pretty-printed tree visualization with Unicode characters
- 📂 Smart sorting with directories listed first
- 🔍 Customizable ignore patterns for excluding directories
- 📋 Clean, readable output format
- 🚫 Built-in ignores for common development folders (.git, __pycache__, etc.)

## Installation

```bash
# Clone the repository
git clone https://github.com/benjamincoad/dtree.git

# Make the script executable
chmod +x dtree
```

## Usage

```bash
# Basic usage (current directory)
./dtree

# Specify a directory
./dtree /path/to/directory

# Ignore specific patterns
./dtree --ignore node_modules .git temp_files

# Full command format
./dtree [path] [--ignore pattern1 pattern2 ...]
```

Example output:
```
Directory Tree for: /my_project

└── my_project
    ├── docs
    │   ├── api.md
    │   └── usage.md
    ├── src
    │   ├── __init__.py
    │   └── main.py
    ├── tests
    │   └── test_main.py
    ├── .gitignore
    └── README.md
```

## Command Line Options

- `path`: Directory to visualize (default: current directory)
- `-i, --ignore`: Patterns to ignore (default: [".git", "__pycache__", ".venv", "node_modules"])

## How It Works

1. Recursively traverses the specified directory
2. Filters out ignored patterns
3. Sorts items (directories first, then files)
4. Generates Unicode-based tree visualization
5. Handles permission errors gracefully

## Use Cases

- Project documentation
- Codebase exploration
- Directory structure planning
- File system visualization
- Documentation generation

## License

MIT License - feel free to use and modify as needed!

## Contributing

Contributions are welcome! Feel free to submit issues and pull requests.
