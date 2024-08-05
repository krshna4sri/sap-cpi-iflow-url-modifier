# SAP CPI IFlow URL Modifier

This repository provides a Python-based solution for automating the export of SAP Cloud Platform Integration (CPI) IFlows, modifying URLs in the OData sections, and managing these operations through a Command Line Interface (CLI).

## Features

- **Export IFlows**: Extracts 50+ IFlows from SAP CPI.
- **URL Modification**: Automatically changes URLs in the OData sections of the exported IFlows.
- **Command Line Interface**: Provides a user-friendly CLI for executing the export and modification processes.
- **Configuration Management**: Uses JSON files for easy configuration of SAP CPI settings and URL replacements.

## Installation

1. **Clone the Repository**
   ```bash
   git clone https://github.com/yourusername/sap-cpi-iflow-url-modifier.git
   cd sap-cpi-iflow-url-modifier
   ```

2. **Install Dependencies**
   Ensure Python and required packages are installed:
   ```bash
   pip install -r requirements.txt
   ```

3. **Setup Configuration**
   - Update `config/config.json` with SAP CPI credentials and settings.
   - Update `config/urls.json` with the old and new URLs for replacement.

## Usage

### Command Line Interface

The CLI provides a simple interface for managing the IFlow export and URL modification process.

**Export and Modify IFlows**
```bash
python src/cli.py --action export_and_modify
```

### Automated Shell Script

A shell script is available for automating the entire process.

```bash
./scripts/export_and_modify.sh
```

## Configuration

- **`config/config.json`**: Contains SAP CPI credentials and other necessary settings.
- **`config/urls.json`**: Specifies the old and new URLs for modification.

## Directory Structure

```
sap-cpi-iflow-url-modifier/
├── src/
│   ├── export_iflows.py       # Exports IFlows from SAP CPI
│   ├── modify_iflows.py       # Modifies URLs in OData sections
│   └── cli.py                 # CLI for managing operations
├── config/
│   ├── config.json            # SAP CPI credentials and settings
│   └── urls.json              # URL replacement settings
├── scripts/
│   ├── export_and_modify.sh   # Shell script for automation
├── README.md                  # Project documentation
├── LICENSE                    # License information
└── .gitignore                 # Git ignore rules
```

## Contributing

Contributions are welcome! Please read the `CONTRIBUTING.md` for guidelines on submitting pull requests.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact

For questions or issues, please open an issue in this repository or contact krshna4sri@gmail.com.
