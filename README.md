# FreeMason9224.dev

Config files for my GitHub profile.

## Table of Contents
- [Introduction](#introduction)
- [Setup](#setup)
- [Usage](#usage)
- [Troubleshooting](#troubleshooting)
- [Security](#security)
- [Contributing](#contributing)
- [Contact](#contact)
- [License](#license)

## Introduction
This repository contains configuration files and workflows for my GitHub profile. It includes scripts and automation tools to manage and secure my projects.

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
3. Set up a virtual environment:
   ```sh
   python3 -m venv env
   ```
4. Activate the virtual environment:
   - On Windows:
     ```sh
     .\env\Scripts\activate
     ```
   - On macOS and Linux:
     ```sh
     source env/bin/activate
     ```
5. Install dependencies:
   ```sh
   pip install -r requirements.txt
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

### Examples
Here are some examples of how to use the secure storage workflow in different scenarios:

- **Encrypting a file:**
  ```sh
  gpg --output encrypted_file.txt --encrypt --recipient $GPG_KEY_ID file_to_encrypt.txt
  ```

- **Decrypting a file:**
  ```sh
  gpg --output decrypted_file.txt --decrypt encrypted_file.txt
  ```

## Troubleshooting
If you encounter any issues, here are some common troubleshooting steps:

- **Virtual environment activation issues:**
  - Ensure you have the correct path to the activation script.
  - Verify that you have the necessary permissions to execute the script.

- **Dependency installation errors:**
  - Check the `requirements.txt` file for any missing or outdated dependencies.
  - Ensure you have an active internet connection to download the dependencies.

## Security
To ensure the security of this repository, follow these best practices:

- Use GitHub Secrets to store sensitive information such as `GPG_PRIVATE_KEY`, `GPG_PASSPHRASE`, and `GPG_KEY_ID`.
- Avoid hardcoding any sensitive information directly in the code or configuration files.
- Regularly rotate secrets and update them in the repository settings.
- Add a security policy to the repository to outline how to report and handle security vulnerabilities.
- Ensure that decrypted secrets are securely cleaned up after use.

## Contributing
Contributions are welcome! Please follow these guidelines when contributing:

- Fork the repository and create a new branch for your changes.
- Ensure your code follows the project's coding standards and passes all tests.
- Submit a pull request with a clear description of your changes.

## Contact
For support or questions, please contact the repository maintainer at [your-email@example.com].

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
