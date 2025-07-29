# TypeDB Drivers

[![Factory](https://factory.vaticle.com/api/status/typedb/typedb-driver/badge.svg)](https://factory.vaticle.com/typedb/typedb-driver)
[![Discord](https://img.shields.io/discord/665254494820368395?color=7389D8&label=chat&logo=discord&logoColor=ffffff)](https://typedb.com/discord)
[![Discussion Forum](https://img.shields.io/discourse/https/forum.typedb.com/topics.svg)](https://forum.typedb.com)
[![Stack Overflow](https://img.shields.io/badge/stackoverflow-typedb-796de3.svg)](https://stackoverflow.com/questions/tagged/typedb)
[![Stack Overflow](https://img.shields.io/badge/stackoverflow-typeql-3dce8c.svg)](https://stackoverflow.com/questions/tagged/typeql)
[![Hosted By: Cloudsmith](https://img.shields.io/badge/OSS%20hosting%20by-cloudsmith-blue?logo=cloudsmith&style=flat)](https://cloudsmith.com)

This repository stores all TypeDB Drivers built and supported by TypeDB.

See the table below for links to README files, documentation, and source code.

| Driver  | Readme                                                                               | Documentation                                                    | Driver location                                                               |
|---------|--------------------------------------------------------------------------------------|------------------------------------------------------------------|-------------------------------------------------------------------------------|
| Rust    | [README](https://github.com/typedb/typedb-driver/tree/master/rust/README.md)   | [Documentation](https://typedb.com/docs/drivers/rust/overview)   | [`rust/`](https://github.com/typedb/typedb-driver/tree/master/rust)     |
| Python  | [README](https://github.com/typedb/typedb-driver/tree/master/python/README.md) | [Documentation](https://typedb.com/docs/drivers/python/overview) | [`python/`](https://github.com/typedb/typedb-driver/tree/master/python) |
| Node.js | [README](https://github.com/typedb/typedb-driver/tree/master/nodejs/README.md) | [Documentation](https://typedb.com/docs/drivers/nodejs/overview) | [`nodejs/`](https://github.com/typedb/typedb-driver/tree/master/nodejs) |
| Java    | [README](https://github.com/typedb/typedb-driver/tree/master/java/README.md)   | [Documentation](https://typedb.com/docs/drivers/java/overview)   | [`java/`](https://github.com/typedb/typedb-driver/tree/master/java)     |
| C       | [README](https://github.com/typedb/typedb-driver/tree/master/c/README.md)      | See C++                                                          | [`c/`](https://github.com/typedb/typedb-driver/tree/master/c)           |
| C++     | [README](https://github.com/typedb/typedb-driver/tree/master/cpp/README.md)    | [Documentation](https://typedb.com/docs/drivers/cpp/overview)    | [`cpp/`](https://github.com/typedb/typedb-driver/tree/master/cpp)       |
| C#      | [README](https://github.com/typedb/typedb-driver/tree/master/csharp/README.md) | [Documentation](https://typedb.com/docs/drivers/csharp/overview) | [`csharp/`](https://github.com/typedb/typedb-driver/tree/master/csharp) |

## Contributing

We welcome contributions to the TypeDB Drivers! This guide will help you get started with contributing to this multi-language driver repository.

### Getting Started

Before contributing, please:

1. **Join the community**: Connect with us on [Discord](https://typedb.com/discord) or the [Discussion Forum](https://forum.typedb.com) to discuss your ideas
2. **Check existing issues**: Browse our [GitHub issues](https://github.com/typedb/typedb-driver/issues) to see if your contribution idea already exists
3. **Read the documentation**: Familiarize yourself with [TypeDB](https://typedb.com/docs) and the specific driver you want to contribute to

### Development Setup

#### Prerequisites

- **Git**: For version control
- **Bazel**: Build system used across all drivers (install from [bazel.build](https://bazel.build/))
- **Language-specific tools**: Depending on which driver you're working on:
  - **Rust**: Install via [rustup](https://rustup.rs/)
  - **Python**: Python 3.7+ and pip
  - **Node.js**: Node.js 14+ and npm
  - **Java**: JDK 11+
  - **C/C++**: GCC or Clang
  - **C#**: .NET 6.0+

#### Setting up the Repository

1. **Fork the repository** on GitHub
2. **Clone your fork**:
   ```bash
   git clone https://github.com/YOUR_USERNAME/typedb-driver.git
   cd typedb-driver
   ```
3. **Add the upstream remote**:
   ```bash
   git remote add upstream https://github.com/typedb/typedb-driver.git
   ```

### Making Changes

#### Branch Naming

Create a descriptive branch name following this pattern:
- `feature/your-feature-name` for new features
- `fix/issue-description` for bug fixes
- `docs/documentation-update` for documentation changes

#### Development Workflow

1. **Create a new branch** from the latest `master`:
   ```bash
   git checkout master
   git pull upstream master
   git checkout -b feature/your-feature-name
   ```

2. **Make your changes** in the appropriate driver directory (`rust/`, `python/`, `nodejs/`, etc.)

3. **Follow language-specific conventions**:
   - Check the individual driver READMEs for specific coding standards
   - Use the existing code style and patterns
   - Include appropriate tests for your changes

#### Building and Testing

Each driver has its own build and test procedures. Generally:

- **Build**: Use Bazel or the language-specific build tools
- **Test**: Run the full test suite before submitting
- **Check**: Ensure your code passes linting and formatting checks

For specific instructions, refer to the README in each driver directory.

### Submitting Your Contribution

#### Before Submitting

1. **Test thoroughly**: Ensure all tests pass and your changes work as expected
2. **Update documentation**: Include relevant documentation updates
3. **Check code style**: Follow the project's coding conventions
4. **Commit with clear messages**: Write descriptive commit messages

#### Pull Request Process

1. **Push your branch** to your fork:
   ```bash
   git push origin feature/your-feature-name
   ```

2. **Create a Pull Request** on GitHub with:
   - **Clear title**: Summarize your changes concisely
   - **Detailed description**: Use our PR template to describe:
     - Usage and product changes
     - Implementation details
   - **Link related issues**: Reference any related GitHub issues

3. **Respond to feedback**: Address review comments promptly and professionally

#### PR Requirements

- All tests must pass
- Code must follow project conventions
- Documentation must be updated if applicable
- PR must be approved by maintainers (see [CODEOWNERS](.github/CODEOWNERS))

### Types of Contributions

We welcome various types of contributions:

- **🐛 Bug Reports**: Use our [bug report template](.github/ISSUE_TEMPLATE/BUG_REPORT.md)
- **✨ Feature Requests**: Use our [feature request template](.github/ISSUE_TEMPLATE/FEATURE_REQUEST.md)
- **🔧 Code Contributions**: Bug fixes, new features, performance improvements
- **📚 Documentation**: Improvements to READMEs, code comments, or guides
- **🎯 New Language Drivers**: Use our [language driver request template](.github/ISSUE_TEMPLATE/LANGUAGE_DRIVER_REQUEST.md)

### Community Guidelines

- **Be respectful**: Treat all community members with respect and kindness
- **Be collaborative**: Work together and help each other
- **Be patient**: Maintainers and contributors are volunteers
- **Follow the code of conduct**: Maintain a welcoming environment for everyone

### Getting Help

If you need help or have questions:

- **Discord**: Join our [Discord server](https://typedb.com/discord) for real-time chat
- **Forum**: Post on our [Discussion Forum](https://forum.typedb.com) for detailed discussions
- **Issues**: Create a GitHub issue for bug reports or feature requests
- **Stack Overflow**: Use tags `typedb` or `typeql` for technical questions

### License

By contributing to TypeDB Drivers, you agree that your contributions will be licensed under the same license as the project (see [LICENSE](LICENSE)).

---

Thank you for contributing to TypeDB Drivers! 🎉

### Package hosting

Package repository hosting is graciously provided by  [Cloudsmith](https://cloudsmith.com).
Cloudsmith is the only fully hosted, cloud-native, universal package management solution, that
enables your organization to create, store and share packages in any format, to any place, with total
confidence.
