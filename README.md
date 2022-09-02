# XML Linter
This tool has a GNU GPLv3 license, please read for information regarding permissions, conditions and limitations of using this software.

This XML linter sorts XML documents alphabetically by tag, whilst respecting parent-child hierarchy and retaining the position of namespace tags in the tree.

### Requirements
- Python 3.4+ Installed in the environment you wish to run this, whether local or virtual.
- In addition to Python the [lxml](https://lxml.de/installation.html) package is required
```
pip install lxml
```

## Linter Arguments

| Flag     | Name  | Description |
| -------- | ----- | ----------- |
| -c       | check | Expects a file or directory path to perform a check for sorting and outputs any unsorted documents and/or XML syntax errors to terminal |
| -w       | write | Expects a file or directory path to format and outputs any linted documents and/or XML syntax errors to terminal |
| -h       | help  | Display information about the optional arguments |




