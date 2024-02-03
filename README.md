# Project-Management-and-Automation
A collection of scripts designed to streamline various tasks related to project configuration, package management, virtual environment activation, directory organization, and script generation.

# Script Repository for Project Management and Automation

Welcome to the Project Management and Automation script repository! This collection of scripts is designed to streamline various tasks related to system configuration, package management, virtual environment activation, directory organization, and script generation. Below is an overview of each script:

## [ls_dpkg.py](https://gist.github.com/AJeschor/a66af7516298adb39efeb21478ebdfe6)
The `ls_dpkg.py` script extracts and formats information about installed Debian-based system packages using the `dpkg --list` command. Users can choose output formats such as Markdown, CSV, YAML, TXT, or XLSX. The script prompts users to specify an output format and directory for saving the resulting file. If Pandas is installed, it is utilized for XLSX format; otherwise, a warning is issued. The default output directory is the user's home directory, and the script ensures the provided directory path is valid.

## [activate_env.py](https://gist.github.com/AJeschor/8be08c8868018a05e31f6b9bd9edc2dc)
The `activate_env.py` script streamlines virtual environment activation in projects with multiple coexisting environments. It identifies and presents virtual environment options within a directory, allowing users to easily select which environment to activate. This script is most effective when employed as a sourced script through an alias for seamless integration into the command line environment.

## [config_dir_gen.py](https://gist.github.com/AJeschor/b684667fc6ab95e3a3531370776c9940)
The `config_dir_gen.py` Python script creates an INI configuration file for project directories, reflecting the directory structure under the current working directory. It categorizes directories into base, terminal, and section directories. The script utilizes configparser and can work as an alias. It defines constants, includes functions for directory manipulation, and generates an INI file for easy configuration management.

## [whichenv.sh](https://gist.github.com/AJeschor/cdb9bef2c0eb7a6230190e8e66fc77e3)
The `whichenv.sh` script detects Poetry, Pipenv, Virtualenv, Conda, and Pyenv environments within a directory. It initializes variables, checks for package manager/tool existence, determines the active state, and prints name and path information about the active environment. The script is designed to assist users in projects with multiple virtual environments, providing details on the active environment.

## [init-gen.py](https://gist.github.com/AJeschor/ddc8454fca7bbb059cdf8bb98c1129f3)
The `init-gen.py` Python script automates the generation of an `__init__.py` file in a directory based on unique non-internal function and class names found in Python files within the same directory. This script enhances code organization by creating import statements in the `__init__.py` file.

Feel free to explore and utilize these scripts to enhance your system management and automation workflows. If you have any questions or feedback, please don't hesitate to reach out.
