# WordPress\_on\_RaspberryPi

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Platform: Raspberry Pi 4](https://img.shields.io/badge/Platform-Raspberry%20Pi%204-green.svg)](#)
[![Stack: LAMP](https://img.shields.io/badge/Stack-LAMP-orange.svg)](#)

## Description

Automate the deployment of a full LAMP stack (Linux, Apache, MariaDB, PHP) on a Raspberry Pi 4 to run WordPress. This repository provides Bash scripts to install and configure each component, delivering a repeatable, self-hosted CMS solution.

## Table of Contents

* [Features](#features)
* [Prerequisites](#prerequisites)
* [Installation](#installation)
* [Usage](#usage)
* [Project Structure](#project-structure)
* [Tools Used](#tools-used)
* [Contributing](#contributing)
* [License](#license)

## Features

* One-click setup via Bash scripts for:

  * Apache HTTP Server
  * PHP (with required extensions for WordPress)
  * MariaDB database server
* Sample configuration files for easy customization
* Troubleshooting guide for common issues

## Prerequisites

* **Hardware:** Raspberry Pi 4 Model B (2GB RAM or higher)
* **OS:** Raspberry Pi OS (32-bit)
* **Network:** Internet access for package downloads
* **Access:** SSH or direct terminal access with `sudo` privileges

## Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/<your-org>/WordPress_on_RaspberryPi.git
   cd WordPress_on_RaspberryPi
   ```
2. **Make scripts executable**

   ```bash
   chmod +x scripts/*.sh
   ```
3. **Run the bootstrap script**

   ```bash
   sudo ./scripts/bootstrap.sh
   ```

## Usage

1. Navigate to your Pi’s IP address in a web browser.
2. Complete the WordPress web installer (site title, admin user, etc.).
3. Secure your site and start publishing content!

## Project Structure

```text
WordPress_on_RaspberryPi/
├── scripts/                 # Installation and configuration scripts
│   ├── install-apache.sh
│   ├── install-php.sh
│   └── install-mariadb.sh
├── config/                  # Sample config files for services
│   ├── apache-vhost.conf
│   ├── php.ini
│   └── wp-config.php.template
├── docs/                    # Documentation and troubleshooting
│   ├── troubleshooting.md
│   └── reference-links.md
├── LICENSE                  # MIT License
└── README.md                # Project overview and setup
```

## Tools Used

* **Bash** for scripting automation
* **Apache** HTTP Server 2.4+
* **PHP** 7.4+ with PDO/MySQL extension
* **MariaDB** 10.3+
* **Raspberry Pi OS** (32-bit)

## Contributing

Contributions are welcome! Please open an issue or submit a pull request with improvements.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
