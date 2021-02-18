![](http://i.imgur.com/AMGwFll.png) **MODS - My Own DSM Shortcuts Packager for Synology**

This project has been created as a workaround for the lack of “Custom Shortcut on Synology Desktop”.

It was first aimed at opening URL’s in new Tabs. It has next been extended to run Shell Scripts and to open web pages (php or html) in floating popup windows on DSM’s desktop.

Finally, it has been completed with support to create actual packages for Synology (.spk), embedding web applications and custom installation wizards and scripts.

Mods is a Windows Application.

![](https://i.imgur.com/MZsNOSV.png)

Packages created with Mods can add several shortcuts in DSM’s menu to open URLs, WebApps or Shell Scripts:

-   Urls can be either “relative paths” to websites hosted on the Synology itself or “absolute Uri’s” of any websites hosted on Internet. Clicking on their icons will open the related URL’s in a new browser tab.
-   Shell Scripts are executed by Synology and their outputs are displayed in real time in popup windows (iFrames) on DSM’s Desktop
-   WebApps (set of php and html pages) are embedded in the package and deployed into the Synology. They are also opened in popup windows (iFrames) on DSM’s Desktop.

WebApps or Shell Scripts are only available since the CTP 4.

In addition, one can configure the Package with start/stop scripts, pre/post-install, uninstall and upgrade scripts, as well as install, upgrade and uninstall wizards UI.

 

Each shortcut can be configured with a custom “title” and “icon”.

Notice:

-   DSM’s context data (like “current user”) cannot be passed as parameters on the URL. The URLs are static.
-   The Web Station and the third party package [Init 3rd Party](https://www.cphub.net/?id=40&pid=5) are not mandatory anymore (See [use of a CGI router](https://github.com/vletroye/SynoPackages/wiki/DSM-CGI-Router-6.x)).
-   Packages created with Mods are only tested on my DS1815+ with DSM 6.x and my DS214play with DSM 7.x)

Here bellow, a shortcut to my blog has been added in DSM’s main menu. I did next drag & drop it onto DSM’s desktop to create a shortcut there.

![](http://i.imgur.com/zGddwbw.png)

 

here is next an icon which executes a simple Shell Command ‘ps -gaceux’ has been added on DSM’s desktop

![](http://i.imgur.com/wnWR5Vx.png)

 

Here is the free web application [php Server Monitor](https://www.phpservermonitor.org) deployed within DSM via a Package made with Mods, and displayed in a popup/floating window. 

![](http://i.imgur.com/G3F775E.png?1)


Here is the famous [Web Console](http://www.web-console.org) running in a popup window of the DSM

![](http://i.imgur.com/Q5pqh9S.png)

All those spk samples are available [here](https://github.com/vletroye/SynoPackages)
