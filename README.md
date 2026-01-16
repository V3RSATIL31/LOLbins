# Living Off The Land Binaries and Scripts (and now also Libraries)

<p align="center">
  <img src="https://img.shields.io/badge/LOLBins-Documentation-blue" alt="LOLBins Documentation"/>
</p>

## Overview

The goal of the LOLBins project is to document every binary, script, and library that can be used for Living Off The Land techniques.

This repository serves as a curated collection and documentation of binaries, scripts, and libraries that can be leveraged by security professionals, penetration testers, and red teams for legitimate security testing purposes.

## What are LOLBins?

LOLBins (Living Off The Land Binaries) are legitimate system binaries, scripts, or libraries that can be abused to perform actions beyond their intended purpose. These tools are particularly valuable in security assessments because they:

- Are native to the operating system or come from trusted sources
- Are digitally signed by legitimate vendors
- Can bypass application whitelisting
- Help maintain stealth during security operations

## Criteria

A LOLBin/Lib/Script must:

* Be a signed file by a legitimate vendor, either native to the OS or downloadable from official sources
* Have extra "unexpected" functionality that goes beyond its intended use case
  * Exceptions include application whitelisting bypasses
* Have functionality that would be useful to security professionals, penetration testers, or red teams

Interesting functionality can include:

* **Executing code**
  * Arbitrary code execution
  * Pass-through execution of other programs (unsigned) or scripts (via a LOLBin)
* **Compiling code**
* **File operations**
  * Downloading files
  * Uploading files
  * Copying files
* **Persistence mechanisms**
  * Pass-through persistence utilizing existing LOLBin
  * Persistence techniques (e.g., hide data in ADS, execute at logon)
* **UAC bypass**
* **Credential operations**
  * Credential theft
  * Dumping process memory
* **Surveillance**
  * Keylogger capabilities
  * Network tracing
* **Log evasion/modification**
* **DLL side-loading/hijacking** without relocation in the filesystem

## Project Structure

```
LOLbins/
├── README.md
├── CONTRIBUTING.md
├── LICENSE
├── YML-Template.yml
├── CategoryList.md
└── yml/
    ├── OSBinaries/
    ├── OSScripts/
    └── OSLibraries/
```

## Contributing

If you have found a new LOLBin, LOLScript, or LOLLibrary that you would like to contribute, please review the contributing guidelines located in [CONTRIBUTING.md](CONTRIBUTING.md).

A template for the required YML format has been provided in [YML-Template.yml](YML-Template.yml).

## Categories

The following categories are used to classify functionality:

* **Execute** - Execute arbitrary code or commands
* **Download** - Download files from remote sources
* **Upload** - Upload files to remote destinations
* **Compile** - Compile code on the target system
* **Copy** - Copy files
* **Persistence** - Establish persistence mechanisms
* **UAC Bypass** - Bypass User Account Control
* **Credentials** - Access or dump credentials
* **Recon** - Perform reconnaissance
* **AWL Bypass** - Application Whitelisting bypass
* **Encode** - Encode data or files
* **Decode** - Decode data or files
* **ADS** - Alternate Data Stream operations

## Usage & Disclaimer

This project is intended for **educational and authorized security testing purposes only**. The information provided here should only be used in environments where you have explicit permission to conduct security assessments.

**Warning**: Misuse of the techniques documented in this repository may violate laws and regulations. Users are solely responsible for ensuring their actions comply with applicable laws and organizational policies.

## Common Hashtags

* #LOLBin
* #LOLBins
* #LOLScript
* #LOLScripts
* #LOLLib
* #LOLLibs

## History

The phrase "Living off the land" was coined by Christopher Campbell (@obscuresec) & Matt Graeber (@mattifestation) at DerbyCon 3.

The term LOLBins came from a Twitter discussion on what to call binaries that can be used by an attacker to perform actions beyond their original purpose.

## License

This project is licensed under the GPL-3.0 License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements

This project is inspired by the excellent work of the [LOLBAS-Project](https://github.com/LOLBAS-Project/LOLBAS) and aims to provide a comprehensive resource for security professionals.
