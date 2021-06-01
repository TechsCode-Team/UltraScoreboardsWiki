# Proxy Installation

There are a variety of proxies out there. BungeeCord is the usual one that is most commonly used, although Waterfall and Travertine (by the Paper devs) are improved for performance. Therefore we recommend [Waterfall](https://papermc.io/downloads#Waterfall), and, if your server supports 1.7.10 (although our plugins don't), use [Travertine](https://papermc.io/downloads#Travertine) instead.
<br>
For a proxy installation you need to repeat the Spigot installation process for every server. Once you have finished installing the plugin on all the back-end servers we need to install it on to the proxy.
Once the plugin has been installed on the proxy we need to setup the MySQL connections inside the back-end servers. <br>

## Connecting to MySQL
<br>

To connect your server to MySQL you need to join your server and use ***/uboard >> settings >> MySQL Database >> Setup MySQL >> credentials***. Here you need to fill in the credentials *(info)* of your database. Once you have filled in all the credentials you can now test the connection and confirm it.
When you have connected a plugin to MySQL you need to restart your server.
When you have repeated this procces for all of your servers your plugin is now proxy ready.
***Note:*** *If your database has not been connected or the test is taking to long you have entered the wrong credentials.*<br>

### Troubleshooting guide
<br>
**My plugin is not connected to MySQL.**
If your plugin is not connecting to MySQL or is taking to long to test the connection if means that you have filled in the wrong credentials, or haven't setup your MySQL correctly on your hosting provider's end.<br>

**Proxy isn't connected.**
If your proxy isn't connected you need to do it manually.
First we need the MySQL key from a connected server. This can be found in there *\SERVER_DIRECOTRY\plugins\Ultra_Scoreboards*. Here you need to copy the MySQL key.
***NOTE:*** *This key can coninue on a second line, so make sure to copy it all!*
