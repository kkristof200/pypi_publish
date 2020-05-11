# pypi_publish

## Setup
1. open .pypirc and add your username and password
2. move .pypirc to $HOME (probably ~/)
3. move pypi_publish to /usr/local/bin (or any  other forder added to your $PATH)

## IMPORTANT
__YOU NEED TO BE IN THE FOLDER, WHERE THE PACKAGE IS LOCATED, TO RUN THIS.__

__THIS PERFORMS THE 'rm' COMMAND, SO IF YOU'RE IN ANOTHER FOLDER, IT MIGHT CAUSE SOME PROBLEMS BY DELETING FODLERS (named dist or build)__

~~~~
enclosing_folder/
|   package_name/
|   |   __init__.py
|   |   anything.py
|   setup.py
|   ...
|   <-- YOU NEED TO RUN FROM THIS FOLDER (enclosing_folder)
~~~~

## Usage
1. Set new version number in setup.py
2. Open up terminal and __ensure you're in the folder where the package is located__ (type 'pwd' to print current folder)
3. type
~~~~Bash
pypi_publish
~~~~

## Notes
to find out your path, type
~~~~Bash
echo $PATH
~~~~
to find out your home, type
~~~~Bash
echo $HOME
~~~~
