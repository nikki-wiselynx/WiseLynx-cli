# WiseLynx

Hardware intelligence layer for Fedora Linux. Scan your system, track changes, and contribute to a community hardware compatibility database.

[![License: AGPL v3](https://img.shields.io/badge/License-AGPL%20v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
[![Python Version](https://img.shields.io/badge/python-3.9%2B-blue)](https://www.python.org/)
[![Build Status](https://img.shields.io/github/actions/workflow/status/wiselynx/cli/test.yml)](https://github.com/wiselynx/cli/actions)

---

## Quick Start

```bash
# Install from source
git clone https://github.com/wiselynx/cli.git
cd cli
pip install -e .

# Scan your system
wiselynx scan -- my-first-scan

# See what changed after an update
wiselynx diff my-first-scan current

$ wiselynx diff before-upgrade after-upgrade
Added: USB camera (046d:0825)
Removed: Intel WiFi (8086:3165)
Storage changed: 500GB -> 1TB (drive replaced)

---

## Commands

# Preview your system
wiselynx preview

# Save a baseline before making changes
wiselynx scan -- before-upgrade

# After updates, see what changed
wiselynx diff before-upgrade current

# List all saved scans
wiselynx list
---

## Contributing

#We welcome contributions of all kinds. See CONTRIBUTING.md for guidelines.

-Report bugs: GitHub Issues
-Suggest features: GitHub Discussions
-Submit changes: Pull Requests
-Share scans for community intelligence - once compatability matrix is live

---

## Root Access

  #Without root, you still get CPU, memory, PCI, USB, and storage information.

---

## Requirements
-Python 3.9 or higher (included with Fedora)
-Fedora Linux (Workstation, Server, IoT, CoreOS)
-Root not required, but provides more detailed hardare info

---

## License
# This program is free software: you can redistribute it and/or modify
# it under the terms of the GNU Affero General Public License as
# published by the Free Software Foundation, either version 3 of the
# License, or (at your option) any later version.
#
# This program is distributed in the hope that it will be useful,
# but WITHOUT ANY WARRANTY; without even the implied warranty of
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
# GNU Affero General Public License for more details.
#
# You should have received a copy of the GNU Affero General Public License
# along with this program. If not, see <https://www.gnu.org/licenses/>.
