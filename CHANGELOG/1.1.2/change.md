Security Updates
* Updated urllib3 from 2.3.0 → 2.5.0 (CVE-2024-37891)
* Updated requests from 2.31.0 → 2.32.4 (CVE-2024-35195)
* Updated setuptools from 40.5.0 → 78.1.1 (CVE-2024-6345)
* Updated Scrapy from 2.12.0 → 2.13.3 for compatibility

Added Features
* Added URL validation with automatic scheme detection
* Integrated security_config.py for ethical testing configuration
  - Default 1 second delay between requests
  - Transparent user agent and headers (X-Scanner, X-Purpose)
  - Configurable robots.txt compliance (default: enabled)
  - Rate limiting with max depth (3) and page count (100)
* New CLI options:
  - `--respect-robots` to enforce robots.txt compliance
  - `--delay <seconds>` to customize request delays

Code Quality
* Removed unused imports (mellisa.py)
* Added comprehensive docstrings to security functions
