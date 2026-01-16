# Contributing to LOLBins

First of all, thank you for considering contributing to LOLBins! This project thrives on community contributions and your expertise is valuable.

## How to Contribute

### 1. Before You Start

- Check if the binary/script/library you want to document already exists in the repository
- Ensure it meets the [criteria listed in the README](README.md#criteria)
- Gather all necessary information about the binary, including:
  - Commands that demonstrate unexpected functionality
  - Operating system versions where it's available
  - Paths where it can be found
  - Detection methods and IOCs
  - Research links and resources

### 2. Use the Template

All submissions must follow the format specified in [YML-Template.yml](YML-Template.yml). This ensures consistency across the documentation.

### 3. Required Fields

At minimum, your submission must include:

- **Name**: The name of the binary/script/library
- **Description**: What it's intended purpose is
- **Author**: Your name (the person documenting this)
- **Created**: Date in YYYY-MM-DD format
- **Commands**: At least one command demonstrating abuse potential
  - **Command**: The actual command syntax
  - **Description**: What the command does
  - **Usecase**: Security testing use case
  - **Category**: From the approved list (Execute, Download, Upload, etc.)
  - **Privileges**: Required privilege level
  - **MitreID**: Relevant MITRE ATT&CK technique
  - **OperatingSystem**: Where this works
- **Full_Path**: At least one path where the binary can be found
- **Acknowledgement**: Credit to researchers who discovered this technique

### 4. Optional but Recommended Fields

- **Aliases**: Alternative names for the same binary
- **Code_Sample**: Links to working examples
- **Detection**: IOCs, Sigma rules, Elastic rules, Splunk detections
- **Resources**: Links to blog posts, research papers, tweets

### 5. File Placement

Place your YML file in the appropriate directory:

- **OSBinaries**: For executables and binaries
- **OSScripts**: For scripts (.ps1, .vbs, .js, etc.)
- **OSLibraries**: For DLLs and libraries

Name the file after the binary/script/library (e.g., `Certutil.yml`, `Powershell.yml`)

### 6. Submission Process

1. Fork this repository
2. Create a new branch for your contribution
3. Add your YML file(s)
4. Ensure the YAML is valid (you can use online YAML validators)
5. Submit a Pull Request with:
   - Clear title describing what you're adding
   - Brief description of the technique
   - Links to any research or proof of concept

### 7. Review Process

- All submissions will be reviewed by maintainers
- We may ask for clarification or additional information
- Once approved, your contribution will be merged

## Quality Guidelines

- **Accuracy**: All information must be accurate and verifiable
- **Clarity**: Write clear, concise descriptions
- **Completeness**: Include as much relevant information as possible
- **Ethics**: Remember this is for authorized security testing only

## Categories

Use one of these approved categories:

- **Execute**: Arbitrary code execution
- **Download**: Download files
- **Upload**: Upload files  
- **Compile**: Compile code
- **Copy**: Copy files
- **Persistence**: Establish persistence
- **UAC Bypass**: Bypass User Account Control
- **Credentials**: Access/dump credentials
- **Recon**: Reconnaissance
- **AWL Bypass**: Application Whitelisting bypass
- **Encode**: Encode data
- **Decode**: Decode data
- **ADS**: Alternate Data Streams

## Example

See existing entries in the `yml/` directory for examples of well-documented LOLBins.

## Questions?

If you have questions about contributing, feel free to open an issue for discussion.

## Code of Conduct

- Be respectful and professional
- Provide constructive feedback
- Remember that contributors are volunteers
- Help maintain a welcoming community

Thank you for helping make LOLBins a valuable resource for the security community!
