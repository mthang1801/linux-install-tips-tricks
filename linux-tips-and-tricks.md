# LINUX TIPS AND TRICKS
1. How to create a desktop shortcut [duplicate]

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;You have to install `gnome-panel` package which comes up with ability to create a application launcher on the desktop or wherever you like. Add `--no-install-recommends` suffix to prevent other package that aren't necessary.
  ```
    $ sudo apt-get install --no-install-recommends gnome-panel
  ```
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;After installing gnome-panel, use following command to create a launcher.
  ```
    $ gnome-desktop-item-edit --create-new ~/Desktop
  ```
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Once you execute the above command, create launcher application will be opened.

  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;![CreateLauncher](https://i.stack.imgur.com/SIJJr.png)
  * In **Type field** "Application" will be a default value. If you're creating launcher for application which has no gui, that runs in terminal like VIM editor then you need to select "Application in Terminal".
  * In **Name field** type application name.
  * In **Command field** type the executable command which open your application.
  * **Comment field** is optional.
  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;To set icon, click on the small box on the top left side near name field and choose a image for it. Click "OK" if you are done.
