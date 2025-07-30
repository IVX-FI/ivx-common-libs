# IVX Common Libraries

Welcome to the IVX Common Libraries repository! This is a centralized collection of shared resources, tools, and libraries used across all IVX projects.

## 🎯 Purpose

This repository serves as a central hub for:
- **Reusable GitHub Actions** for CI/CD workflows
- **Shared Node.js packages** and utilities(_coming soon_)
- **Common configuration files** (ESLint, Prettier, TypeScript configs)(_coming soon_)
- **Documentation templates** and standards(_coming soon_)
- **Build tools** and scripts(_coming soon_)
- **Testing utilities** and helpers(_coming soon_)

## 📁 Repository Structure

```
├── .github/
│   ├── workflows/          # Reusable GitHub Actions workflows
│   └── actions/            # Custom GitHub Actions
└── packages/
```

## 🚀 Getting Started

### For GitHub Actions

To use the shared GitHub Actions in your project:

```yaml
# In your project's .github/workflows/ci.yml
name: CI
on: [push, pull_request]

jobs:
  test:
    uses: IVX-FI/ivx-common-libs/.github/workflows/test.yml@main
    with:
      node-version: '18'
```

## 🔧 Available GitHub Actions

### Build and Deploy Action
Builds and deploys applications to various environments.

```yaml
uses: IVX-FI/ivx-common-libs/.github/action/CI/containerize.yml@main
```

## 🤝 Contributing

We welcome contributions from all IVX team members and external members!

### Quick Start for Contributors

1. **Fork the repository**
2. **Create a feature branch**
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. **Make your changes**
4. **Run tests**
   ```bash
   npm test
   ```
5. **Submit a pull request**

## 📋 Requirements

- Node.js >= 16.0.0
- npm >= 8.0.0 or yarn >= 1.22.0
- Git >= 2.20.0

## 🏷️ Versioning

This project follows [Semantic Versioning](https://semver.org/).

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🆘 Support

For questions, issues, or feature requests:

- **Create an issue** in this repository
- **Contact the IVX team** via Telegram or Discord

---

Made with ❤️ by the IVX Team