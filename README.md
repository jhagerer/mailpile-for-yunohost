# About #

This should become an application package to install [Mailpile](https://www.mailpile.is) on a [Yunohost](https://yunohost.org/) server instance.

Please note that this is under development and **not working** at all right now.


# Done #

- Installation and update scripts according to the [Mailpile documentation](https://github.com/mailpile/Mailpile/wiki/Getting-started-on-Linux).
    - The installation script checks out the current master branch of Mailpile on Github, create a virtualenv around it, and starts the whole thing.
    - These scripts only work when executed locally via ```bash install``` etc. They do not adhere to the Yunohost application package standard yet.


# TODOs #

- Include a systemd configuration file
- Make the installation user specific
- Provide nginx server configuration files

Check this [Yunohost example package](https://yunohost.org/#/packaging_apps).
