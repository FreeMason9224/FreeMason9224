# FreeMason9224.dev

Config files for my GitHub profile.

## Table of Contents
- [Introduction](#introduction)
- [Setup](#setup)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Introduction
This repository contains configuration files and workflows for my GitHub profile. It includes scripts and automation tools to manage and secure my projects. The purpose of this repository is to provide a centralized location for managing and automating various tasks related to my GitHub projects, ensuring consistency and security across all repositories.

## Setup
To set up the project locally:
1. Clone the repository:
   ```sh
   git clone https://github.com/FreeMason9224/FreeMason9224.dev.git
   ```
2. Navigate to the project directory:
   ```sh
   cd FreeMason9224.dev
   ```

## Usage
### Secure Storage Workflow
This workflow ensures that sensitive information is securely handled and cleaned up following its use.

To run the secure storage workflow:
1. Ensure you have the required secrets set in your repository settings:
   - `GPG_PRIVATE_KEY`
   - `GPG_PASSPHRASE`
   - `GPG_KEY_ID`

2. The workflow will automatically run on pushes and pull requests to the `main` branch.

### Automated Testing
This repository includes a workflow for automated testing using `pytest`. The tests are run automatically on pushes and pull requests to the `main` branch.

To run the tests locally:
1. Ensure you have `pytest` installed:
   ```sh
   pip install pytest
   ```
2. Run the tests:
   ```sh
   pytest
   ```

## Contributing
Contributions are welcome! Please open an issue or submit a pull request for any improvements.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
