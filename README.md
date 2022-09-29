# XML Linter
This tool has a GNU GPLv3 license, please read for information regarding permissions, conditions and limitations of using this software.

This linter requires Python 3.4+, it is untested on older versions.
The linter sorts XML documents alphabetically by tag attribute, whilst respecting parent-child hierarchy and retaining the position of namespace tags in the tree.

## Installing Dependencies
- Checkout this repo ```git checkout -- https://github.com/rebeccajan/xml_linter.git```
-  Navigate to the repo folder via CLI and run <br/>
For Windows: ```pip install -r requirements.txt``` <br/>
For Mac: ```pip3 install -r requirements.txt```

### Optional Arguments

| Flag | Name  | Description |
| ---- | ----- | ----------- |
| -a   | anchor| Expects the tag value you wish to anchor at the top of its subset <br/> eg. `<fullName>` would be executed as ```python xml_linter -a fullName``` |
| -c   | check | Expects a file or directory path to perform a check for sorting and outputs any unsorted documents and/or XML syntax errors to terminal |
| -w   | write | Expects a file or directory path to format and outputs any linted documents and/or XML syntax errors to terminal |
| -h   | help  | Display information about the optional arguments |

### Known Limitations
- Escaped special characters are unescaped when a lint write is performed eg."&apos;" will become "'"
- XML files containing comments i.e. "<!--"  will have these removed if sorting is required on write

