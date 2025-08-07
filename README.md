# Fandango Specifications Repository

A curated collection of open-source Fandango grammar specifications for various input formats, designed to facilitate grammar-based fuzzing and testing of programs across different domains.

## 📋 Project Description

This repository serves as a centralized hub for Fandango specification files (`.fan` format) that define grammars for different input formats and protocols. Each specification is accompanied by comprehensive documentation and ready-to-use testing harnesses, making it easy for researchers and developers to perform grammar-based fuzzing on various software systems.

### What is Fandango?

[Fandango](https://fandango-fuzzer.github.io) is a language-based fuzzer that generates test inputs based on formal grammar specifications. This repository provides pre-built grammars and testing infrastructure for common input formats, allowing you to quickly start fuzzing different types of parsers and processors.

## 🗂️ Repository Structure

The repository is organized by subject/format, with each directory containing:

```
subject-name/
├── subject.fan      # Fandango grammar specification file
├── README.md        # Format-specific documentation
└── harness.py       # Python testing harness
```

### Directory Contents

- **`subject.fan`**: The core Fandango grammar specification file defining the syntax rules for the target format
- **`README.md`**: Detailed documentation including:
  - Grammar coverage and features implemented
  - Known limitations and missing features
  - Specific considerations and potential issues
  - Usage examples and testing notes
- **`harness.py`**: A Python script that:
  - Loads the Fandango grammar
  - Generates test inputs using the specification
  - Interfaces with target programs/parsers for testing
  - Handles execution and result collection

## 🚀 Quick Start

### Prerequisites

- Python 3.10+
- Fandango fuzzer installed

### Basic Usage

1. Clone the repository:
```bash
git clone https://github.com/fandango-fuzzer/fandango-specs.git
cd fandango-specs
```

2. Navigate to your desired format:
```bash
cd xml  # or any other format directory
```

3. Run the testing harness:
```bash
python harness.py
```

## 🤝 Contributing

We welcome contributions! Here's how you can help:

### Adding a New Specification

1. Create a new directory named after the format/protocol
2. Implement the three required files:
   - `format.fan` - The grammar specification
   - `README.md` - Documentation and notes
   - `harness.py` - Testing harness
3. Follow the established patterns and documentation standards
4. Test your specification thoroughly
5. Submit a pull request

### Improving Existing Specifications

- Enhance grammar coverage
- Fix bugs or limitations
- Improve documentation
- Optimize testing harnesses
- Add support for more target programs

### Documentation Standards

Each format-specific README should include:
- **Overview**: Brief description of the format
- **Grammar Coverage**: What aspects are implemented
- **Limitations**: Known gaps or missing features
- **Issues**: Documented problems or edge cases
- **Testing Notes**: How to use the harness effectively
- **References**: Relevant specifications or documentation

## 🛠️ Development Guidelines

- **Grammar Quality**: Strive for comprehensive coverage while maintaining clarity
- **Documentation**: Document all decisions, limitations, and known issues
- **Testing**: Include diverse test cases and edge conditions
- **Compatibility**: Ensure harnesses work with common implementations
- **Maintainability**: Write clear, well-commented code

## 📝 License

This project is licensed under the GPL-3.0 License - see the [LICENSE](LICENSE) file for details.

## 🙋‍♀️ Support and Questions

- **Issues**: Report bugs or request features via GitHub Issues
- **Discussions**: Join conversations in GitHub Discussions
- **Documentation**: Check format-specific READMEs for detailed information

---

**Note**: This is an active research project. Specifications may evolve as we discover new edge cases and improve grammar coverage. Always check the format-specific documentation for the latest information.
