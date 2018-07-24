# About #

This should become an application package to install [Mailpile](https://www.mailpile.is) on a [Yunohost](https://yunohost.org/) server instance.

Please note that this is under development and **not working** at all right now.

# How to Set Up #

```
ssh admin@your.yunohost.tld
> git clone https://github.com/ghagerer/mailpile-for-yunohost.git
> cd mailpile-for-yunohost
> bash scripts/install # clone and install Mailpile + dependencies and start it as daemon
```

The current problem is that the running Mailpile Python web server is running on port 33411, which is not reachable through nginx and Yunohost respectively.

# Done #

- Installation and update scripts according to the [Mailpile documentation](https://github.com/mailpile/Mailpile/wiki/Getting-started-on-Linux).
    - The installation script checks out the current master branch of Mailpile on Github, create a virtualenv around it, and starts the whole thing by using a corresponding systemd .service file.
    - These scripts only work when executed locally via ```bash install``` etc. They do not adhere to the Yunohost application package standard yet.


# TODOs #

- Use the Yunohost helper scripts to do the actual installation properly
- Provide parameterized nginx server and systemd.service configuration files

Check this [Yunohost example package](https://yunohost.org/#/packaging_apps).
