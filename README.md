# Nobel Prize App - Pipeline Testing Project

A Node.js web application that displays Nobel Prize winners from the previous 5 years, featuring comprehensive CI/CD pipeline testing with GitHub Actions.

## Features

- Displays Nobel Prize winners from the last 5 years
- Fetches real-time data from the Nobel Prize API
- Responsive web interface
- Advanced GitHub Actions pipeline with multi-OS testing
- Security scanning and code quality checks


![Screenshot (75)](https://github.com/user-attachments/assets/8fadd2d7-ecaa-4873-a2ed-0937a2583f2e)
![Screenshot (74)](https://github.com/user-attachments/assets/f8f8ebc8-248a-4cc4-9919-b59edf7b9ef7)

## Quick Start

### Prerequisites
- Node.js (v16 or higher)
- npm

### Installation

```bash
# Clone the repository
git clone https://github.com/Mide69/NobelApp-Test-Run.git
cd NobelApp-Test-Run

# Install dependencies
npm install

# Start the server
npm start
```

The application will be available at `http://localhost:2000`

## CI/CD Pipeline

This project features an advanced GitHub Actions pipeline that includes:

### Pipeline Jobs

1. **Code Quality** - Syntax validation and dependency checks
2. **Matrix Testing** - Cross-platform testing on Ubuntu, Windows, and macOS with Node.js versions 16, 18, and 20
3. **Security Scanning** - Vulnerability detection using Trivy scanner
4. **Test Summary** - Consolidated status reporting

### Pipeline Features

- **Smart Triggering**: Only runs on relevant file changes
- **Multi-OS Support**: Tests across Ubuntu, Windows, and macOS
- **Node.js Matrix**: Tests multiple Node.js versions
- **Security First**: Automated vulnerability scanning
- **Fail-Fast Strategy**: Optimized for quick feedback

## API Integration

The app integrates with the [Nobel Prize API](https://api.nobelprize.org/) to fetch:
- Prize categories (Physics, Chemistry, Medicine, Literature, Peace, Economics)
- Laureate information
- Award years and details

## Project Structure

```
.
├── .github/
│   └── workflows/
│       └── test.yml          # CI/CD pipeline configuration
├── server.js                 # Main application file
├── package.json              # Dependencies and scripts
├── package-lock.json         # Dependency lock file
├── LICENSE                   # Project license
└── README.md                 # This file
```



## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Ensure all pipeline checks pass
5. Submit a pull request

## License

This project is licensed under the terms specified in the LICENSE file.
