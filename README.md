<h1 align="center">
  <a href="https://github.com/sureserverman/ssh-menu">
    <!-- Please provide path to your logo here -->
    <img src="docs/images/logo.svg" alt="Logo" width="100" height="100">
  </a>
</h1>

<div align="center">
  ssh-menu tools
  <br />
  <a href="#about"><strong>Explore the screenshots »</strong></a>
  <br />
  <br />
  <a href="https://github.com/sureserverman/ssh-menu/issues/new?assignees=&labels=bug&template=01_BUG_REPORT.md&title=bug%3A+">Report a Bug</a>
  ·
  <a href="https://github.com/sureserverman/ssh-menu/issues/new?assignees=&labels=enhancement&template=02_FEATURE_REQUEST.md&title=feat%3A+">Request a Feature</a>
  .
  <a href="https://github.com/sureserverman/ssh-menu/issues/new?assignees=&labels=question&template=04_SUPPORT_QUESTION.md&title=support%3A+">Ask a Question</a>
</div>

<div align="center">
<br />

[![Project license](https://img.shields.io/github/license/sureserverman/ssh-menu.svg?style=flat-square)](LICENSE)

[![Pull Requests welcome](https://img.shields.io/badge/PRs-welcome-ff69b4.svg?style=flat-square)](https://github.com/sureserverman/ssh-menu/issues?q=is%3Aissue+is%3Aopen+label%3A%22help+wanted%22)
[![code with love by sureserverman](https://img.shields.io/badge/%3C%2F%3E%20with%20%E2%99%A5%20by-sureserverman-ff1414.svg?style=flat-square)](https://github.com/sureserverman)

</div>

<details open="open">
<summary>Table of Contents</summary>

- [About](#about)
  - [Built With](#built-with)
- [Getting Started](#getting-started)
  - [Installation](#installation)
- [Usage](#usage)
- [Roadmap](#roadmap)
- [Project assistance](#project-assistance)
- [Authors & contributors](#authors--contributors)
- [Security](#security)
- [License](#license)

</details>

---

## About

> This set of tools was made to simplify and automate some daily tasks of linux administrators. 
> It includes **ssh-menu** for easy ssh access to your servers, **menu-add** for adding servers to your server list for ***ssh-menu*** and
> **menu-rm** for servers removal from the abovementioned list
>
> If you have any ideas about what to add to this set, feel free to create an issue or a pull request

### Built With

> Pure bash and bash only. No strings attached. Thus it can be installed to any debian-based linux distro and any architecture

## Getting Started

### Installation

> `git clone https://github.com/sureserverman/ssh-menu.git`\
> `dpkg-deb --build ssh-menu`\
> `sudo dpkg -i ssh-menu`


## Usage

> `ssh-menu -h` or `ssh-menu --help` - to print help\
> `ssh-menu` without arguments to choose server from the list interactively\
> `ssh-menu servernumber` to connect to the server which has number *servernumber* in your list\
> The list is stored in /etc/ssh-menu/server-list file
> 
> `menu-add -h` or `menu-add --help` - to print help\
> `menu-add argument1 argument2...` with as many arguments as you need\
> where argument could be either name of file, which contains ssh commands\
> that looks like 'ssh -p port user@127.0.0.1 #description'\
> or the command itself in single or double quotes (you can use both types of argument simultaneously)\
> `menu-add` without arguments for interactively entering elements of ssh command
> 
> `menu-rm -h` or `menu-rm --help` - to print help\
> `menu-rm` without arguments for chosing which server to remove interactively\
> `menu-rm servernumber1 servernumber2...` with as many arguments as you need\
> where argument should be number of existing command in the menu

## Roadmap

See the [open issues](https://github.com/sureserverman/ssh-menu/issues) for a list of proposed features (and known issues).

- [Top Feature Requests](https://github.com/sureserverman/ssh-menu/issues?q=label%3Aenhancement+is%3Aopen+sort%3Areactions-%2B1-desc) (Add your votes using the 👍 reaction)
- [Top Bugs](https://github.com/sureserverman/ssh-menu/issues?q=is%3Aissue+is%3Aopen+label%3Abug+sort%3Areactions-%2B1-desc) (Add your votes using the 👍 reaction)
- [Newest Bugs](https://github.com/sureserverman/ssh-menu/issues?q=is%3Aopen+is%3Aissue+label%3Abug)

## Project assistance

If you want to say **thank you** or/and support active development of ssh-menu tools:

- Add a [GitHub Star](https://github.com/sureserverman/ssh-menu) to the project.
- Tweet about the ssh-menu tools.
- Write interesting articles about the project on [Dev.to](https://dev.to/), [Medium](https://medium.com/) or your personal blog.

Together, we can make ssh-menu tools **better**!

## Authors & contributors

The original setup of this repository is by [Serverman](https://github.com/sureserverman).

For a full list of all authors and contributors, see [the contributors page](https://github.com/sureserverman/ssh-menu/contributors).

## Security

ssh-menu tools follows good practices of security, but 100% security cannot be assured.
ssh-menu tools is provided **"as is"** without any **warranty**. Use at your own risk.

_For more information and to report security issues, please refer to our [security documentation](docs/SECURITY.md)._

## License

This project is licensed under the **GPLv3 license**.

See [LICENSE](LICENSE.md) for more information.
