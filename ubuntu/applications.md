# Applications

## apt-get command

    sudo apt-get install vim git vlc flashplugin-installer bleachbit gdebi-core ubuntu-restricted-extras

## Applications and Deb Packages


For deb packages, run `sudo dpkg -i package_name.deb`.
For tar.gz packages, extract them and put them in `/opt`. Then run the installer shell script (usually named `install.sh`).
For run packes, simply run `package_name.run` file and follow the installation wizard instructions.

**In case of dependency errors, run `sudo apt-get -f install`.**

* [Google Chrome](https://www.google.com/chrome/browser/thankyou.html?platform=linux)
* [PyCharm](https://www.jetbrains.com/pycharm/download/#section=linux)
* [CLion](https://www.jetbrains.com/clion/)
* [IntelliJ IDEA](https://www.jetbrains.com/idea/)
* [RStudio](https://www.rstudio.com/products/rstudio/download2/)
* [Sublime Text 3](https://www.sublimetext.com/3)
* [Foxit Reader](https://www.foxitsoftware.com/products/pdf-reader/)
* [Viber](http://www.viber.com/en/products/linux)
* [Skype](https://www.skype.com/en/download-skype/skype-for-linux/downloading/?type=ubuntu64)

## Applications with some installation workarounds

### Dropbox

* Install deb from [here](https://www.dropbox.com/install?os=lnx)
* Run `sudo dpkg -i dropbox_.*.deb`
* In case of unmet dependencies, run `sudo apt-get install -f install`
* [Optional] Install `python-gpgme`, Use `sudo apt-get install python-gpgme`.
* If you haven't configured `HTTP_PROXY` and `HTTPS_PROXY`, configure them.
* Start Dropbox. Use `dropbox start -i`.
* If Dropbox deamon is showing connection error, run `sudo dropbox proxy manual http proxyhost proxy_port username passowrd`. See [this](http://askubuntu.com/a/718794).
* Sign In.

