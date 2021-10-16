# linuxfoundationx-lfw111x
Introduction to Node.js

## Installing Node.js on macOS and Linux
In this section, we will look at installing Node on macOS and Linux. For Windows users feel free to skip to the next section, unless using Windows Subsystem for Linux v2 in which case this section may also be relevant.

The recommended way to install Node.js on macOS and Linux is by using a Node version manager, in particular nvm. We are going to install nvm and then use it to install Node.

The current nvm version is v0.37.2 (as of December 2020), so the install process will contain this version in the URL, if a greater version is out at time of reading, replace v0.37.2 with the current nvm version. For this installation process we assume that Bash, Sh, or Zsh is the shell being used, Fish is not supported but see the nvm readme for alternatives.

The way to install nvm is via the install script at https://github.com/nvm-sh/nvm/blob/v0.37.2/install.sh. If curl is installed (it usually is) a single command can be used to install and setup nvm:

``curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.37.2/install.sh | bash``

If using zsh (e.g. on newer macOS releases) the bash part of the command can be replaced with zsh.

Alternatively the file can be downloaded and saved, and then easily executed like so:

``cat install.sh | bash``

Again bash can be replaced with zsh. To check that the installation was successful execute the following in the terminal:

``command -v nvm``

It should output nvm. If this fails on Linux, close and reopen the terminal (or SSH session) and try running the command again. On macOS see "Troubleshooting on macOS" for in depth troubleshooting.

Now that we have a version manager, let's install the Node version:

``nvm install 14``

This will install the latest version of Node 14:

We can verify that Node is installed, and which version, with the following command:

``node -v``

Congratulations, we now have the right setup on our macOS or Linux machine to proceed.
