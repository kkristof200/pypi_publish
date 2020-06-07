# pypi_publish

## Install
~~~~shell
wget https://raw.githubusercontent.com/kkristof200/pypi_publish/master/pypi_publish -O /usr/local/bin/pypi_publish && chmod u+x /usr/local/bin/pypi_publish
# or
curl https://raw.githubusercontent.com/kkristof200/pypi_publish/master/pypi_publish > /usr/local/bin/pypi_publish && chmod u+x /usr/local/bin/pypi_publish
~~~~

2. Create a file with the name '.pypirc' in your $HOME directory and add your credentials
~~~~
[distutils]
index-servers =
    pypi

[pypi]
username: USERNAME-PROBABLY-__token__
password: PASSWORD
~~~~


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
