# Python Built-in Type Inspector

A comprehensive, interactive tool for exploring and understanding Python's built-in data types. Perfect for beginners learning Python or experienced developers who want a quick reference to built-in type methods.

## Features

- **Detailed Type Analysis** - Explore all methods and attributes of built-in types
- **Categorized Methods** - Methods organized into logical groups:
  - Constructors & Initialization
  - Query Methods (non-mutating)
  - Mutation Methods (modify objects)
  - Conversion Methods
  - Operator Overloads
  - Special/Magic Methods
- **Practical Examples** - Real-world usage examples for each type
- **Type Comparison** - Compare methods between different types
- **Interactive Mode** - Easy-to-use menu-driven interface
- **Method Signatures** - View function signatures and docstrings

## Quick Start

### Installation

Clone the repository:
```bash
git clone https://github.com/s-a-c-h-in/Python-Data-Type-Inspector.git
cd Python-Data-Type-Inspector
```

No additional dependencies required - uses only Python standard library!

### Usage

#### Interactive Mode

Run the inspector interactively:
```bash
python Python-Data-Type-Inspector.py
```

#### Command Line Mode

Analyze a specific type directly:
```bash
python Python-Data-Type-Inspector.py str
python Python-Data-Type-Inspectorr.py list
python Python-Data-Type-Inspector.py dict
```

## Supported Types

The inspector supports all major Python built-in types:

### Numeric Types
- `int` - Integer numbers
- `float` - Floating point numbers
- `complex` - Complex numbers
- `bool` - Boolean values

### Sequence Types
- `str` - Strings
- `list` - Lists
- `tuple` - Tuples
- `range` - Range objects

### Set Types
- `set` - Mutable sets
- `frozenset` - Immutable sets

### Mapping Types
- `dict` - Dictionaries

### Binary Types
- `bytes` - Immutable byte sequences
- `bytearray` - Mutable byte arrays
- `memoryview` - Memory view objects

### Other Types
- `slice` - Slice objects
- `type` - Type objects
- `object` - Base object type

## Usage Examples

### Example 1: Analyzing the `str` Type

```python
$ python builtin_type_inspector.py str
```

Output shows:
- Type information and inheritance chain
- All string methods categorized by purpose
- Method signatures and descriptions
- Practical usage examples

### Example 2: Interactive Exploration

```bash
$ python Python-Data-Type-Inspector.py

WHAT WOULD YOU LIKE TO DO?
  1. Analyze a built-in type
  2. Show practical examples
  3. Inspect a specific method
  4. Compare two types
  5. List all available types
  6. ❌ Exit

➤ Enter your choice (1-6): 1
➤ Enter type name: list
```

### Example 3: Comparing Types

Compare methods between `list` and `tuple`:
```python
inspector.compare_types('list', 'tuple')
```

See which methods are common and which are unique to each type.

### Example 4: Inspecting a Specific Method

```python
inspector.load_type('str')
inspector.inspect_method('split')
```

View detailed documentation and signature for a specific method.

## Menu Options

1. **Analyze a built-in type** - Complete breakdown of a type's methods
2. **Show practical examples** - Copy-paste ready code examples
3. **Inspect a specific method** - Detailed view of a single method
4. **Compare two types** - Side-by-side comparison
5. **List all available types** - View all supported types
6. **Exit** - Close the inspector

## Educational Value

This tool is excellent for:

- **Learning Python** - Understand what methods are available for each type
- **Reference** - Quick lookup of method signatures and usage
- **Teaching** - Demonstrate Python's object-oriented nature
- **Exploration** - Discover lesser-known methods and capabilities

## Code Structure

```
Python-Data-Type-Inspector.py
├── BuiltinTypeInspector (main class)
│   ├── __init__() - Initialize with built-in types
│   ├── list_available_types() - Display all types
│   ├── load_type() - Load a type for inspection
│   ├── analyze_type() - Analyze current type
│   ├── categorize_methods() - Group methods by purpose
│   ├── show_examples() - Display usage examples
│   ├── inspect_method() - Detailed method view
│   ├── compare_types() - Compare two types
│   └── interactive_mode() - Run interactive menu
└── main() - Entry point
```

### Ideas for Contributions

- Add more practical examples for each type
- Support for additional built-in types or modules
- Export functionality (save analysis to file)
- Web interface version
- Comparison of multiple types (3+)
- Performance benchmarking for methods

## Acknowledgments

- Inspired by Python's `help()` and `dir()` functions
- Built with Python's `inspect` module
- Thanks to the Python community for excellent documentation

## Star History

If you find this tool useful, please consider giving it a star 
