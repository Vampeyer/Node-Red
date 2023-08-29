1. Install Node.js
Download the latest LTS version of Node.js from the official Node.js home page. It will offer you the best
 version for your system.

Run the downloaded MSI file. Installing Node.js requires local administrator rights; if you are not a local administrator, you will be prompted for an administrator password on install. Accept the defaults when installing. After installation completes, close any open command prompts
 and re-open to ensure new environment variables are picked up.

Once installed, open a command prompt and run the following command to ensure Node.js and npm are installed correctly.

Using Powershell: node --version; npm --version

Using cmd: node --version && npm --version

You should receive back output that looks similar to:

v18.15.0
9.5.0
2. Install Node-RED
Installing Node-RED as a global module adds the command node-red to your system path.
 Execute the following at the command prompt:

npm install -g --unsafe-perm node-red



3. Run Node-RED
Once installed, you are ready to run Node-RED.

Alternative Installations on Windows
In this section, we provide you with information on alternative ways to install Node.js, npm and the Windows Build Tools needed to install some Nodes for Node-RED on Windows.

Note : You should not use an administrative (a.k.a. "elevated") command prompt unless specifically instructed to. You will very likely need to be quite familiar with command prompts as you learn about Node-RED and Node.js and it will be worth while reading some of the Microsoft articles on PowerShell. the PowerShell Tutorial and PowerShell One-Liners sites may also be helpful.
Standard installations of Node.js on Windows require local administrator rights. Download the appropriate version from the official Node.js home page. It will offer you the best version. While you can use either 32 bit or 64 bit versions on 64 bit Windows, it is recommended to use the 64bit version of Node. If for some reason, you need a different installation, you can use the Downloads Page.

There are two potentially useful alternatives to installing Node.js with the MSI installer.

Using the Chocolatey package manager

Chocolatey is a package manager for Windows similar to APT or yum on Linux and brew on the Macintosh platforms. If you are already using Chocolatey, you may want to use this tool to install Node.js (e.g. using the nodejs-lts package). Note however, that many packages have uncertain management and that these packages may use different folder locations than those mentioned above.

Using a Node version manager

Using a Node.js version manager such as nvm-windows can be very helpful if you are doing Node.js development and need to test against different versions. Keep in mind that you will need to reinstall global packages and may need to re-install local packages when when you switch the version of Node you are using.