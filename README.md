The framework source code can be found here: [cakephp/cakephp](https://github.com/cakephp/cakephp).
## Installation

1. Download [Composer](https://getcomposer.org/doc/00-intro.md)

If Composer is installed globally, run
2. Run `cmd`.
3. Run `composer create-project --prefer-dist cakephp/app:~4.0 my_app_name`.


# cakephp4.4.4
cakePHP 4.44
- GitHub Repository of a Working installation of CakePHP 4.4.4 configured to work on windows 10 running IIS Server or IIS Express
- Simple download the repository, extra to a folder e.g appname
- If you have Visual Studio for Code installed, right click and select Open with Code to open folder. if not Download  [64 bit Windows versionVSCode] (https://code.visualstudio.com/download)
- Install IIS Express extension for VSCode or Download [IIS Express] (https://marketplace.visualstudio.com/items?itemName=warren-buckley.iis-express)
- By Default IIS Express Server is installed on Windows 10.
- Ensure that PHP is installed or Download [VC15 x64 Non Thread Safe] (https://windows.php.net/downloads/releases/php-7.4.30-nts-Win32-vc15-x64.zip)
- Extra content of above downloaded zip file to folder on your PC for example C:\Program Files\PHP\v7.4.3 or C:\PHP\v7.4.3
- Left Click Window Start Icon and Select Run and past %userprofile%\documents\iisexpress\config\applicationhost.config to open applicationhost.config with VSCode
- To enable PHP on IIS Express, update applicationhost.config in (%userprofile%\documents\iisexpress\config\applicationhost.config)
- In the applicationhost.config file search for <fastCgi/> tag entry and replace it with the below, pointing to the directory where your PHP has been installed
	<fastCgi>
		<application fullPath="C:\Program Files\PHP\v7.4.3\php-cgi.exe" />
	</fastCgi>
