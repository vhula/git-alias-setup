# `sgit`

This is a tool for managing git configuration easily

## Table of contents
  * [Table of contents](#table-of-contents)
  * [Installation](#installation)
    * [Manual installation](#manual-installation)
  * [Usage](#usage)
    * [Generic configuration](#generic-configuration)
    * [Alias configuration](#alias-configuration)
      * [Supported aliases](#supported-aliases)
  * [Contributions and Development](#contributions-and-development) 


## Installation

### Manual installation

Follow these steps to install `sgit` manually:
1. clone this repository
2. add `<cloned directory>/scripts` directory to your `$PATH`

    Assuming that this repository cloned into `/usr/local/bin/sgit/` directory:
    
    `export PATH=$PATH:/usr/local/bin/sgit/scripts`
    

## Usage
1. Generic usage

    `$sgit [ARGUMENT VALUE]... [OPTION]...`

2. Help

    `$sgit --help`
    
    ```
    Usage: sgit [ARGUMENT VALUE]... [OPTION]...
    Sets up different aliases for git command
    All options are applied globaly by default (git config --global)
    
    Arguments:
            -u, --username                  name of the user for git env
            -e, --email                     email of the user for git env
            --editor                        git editor
    Options
            -h, --help                      print usage
            -c, --configure                 configure default aliases
            --global-off                    apply configuration for the current user only
    ```

### Generic configuration
1. Configure username:

    `$sgit --username "<Your Name>"`
    
    `$sgit -u "<Your Name>"`
    
2. Configure email:

    `$sgit --email "<Your Email>"`
    
    `$sgit -e "<Your Email>"`
    
  Multiple options can be applied simultaneously:

   `$sgit -u "<Your Name>" -e "<Your Email>" --editor "vim"`

### Alias configuration
1. Configure all supported aliases:

    `$sgit --configure`
    
    `$sgit -c`

#### Supported aliases

(More will be added later)

| Alias      | Command            | Description |
| ---------- | ------------------ | ----------- |
| `s`        | `status`           |             |
| `pr`       | `pull --rebase`    |             |

### Contributions and Development

#### Contribution

1. Create an issue (what you want to see in this tool)
2. Assign any issue to yourself
3. Create a pull request

#### Development

What suites you best :)