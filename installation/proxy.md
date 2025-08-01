# Proxy Installation
Ultra Scoreboards works on every proxy based of **[BungeeCord](https://ci.md-5.net/job/BungeeCord)**. If you use a proxy like **[Waterfall](https://papermc.io/downloads#Waterfall)** or technically every proxy that is forked (based) of either BungeeCord or Waterfall. The plugin should work just fine. Nevertheless, we do recommend using a proxy such as Waterfall, which is more performant and secure than BungeeCord.
<br>

**`Note:`**
While we work on updating the core of our plugins, our plugins currently do not support Velocity or any fork thereof. 
<br>

For a proxy installation, you need to repeat the plugin installation process for every Spigot server that you have. Once you have finished installing the plugin on all the back-end (Spigot/Paper) servers, you need to install it on the proxy.
<br>

The process is similar as the Spigot installation:
<br>

- Shut down your server.
- Upload the plugin.
- Start your server.

`Note:` *You will need a MySQL database to be able to use Ultra Scoreboards in proxy mode. Depending on your host, the process can vary, and will not be mentionned or explained here.*

Once the plugin has been installed on the proxy, and that it's loading as expected, we need to set up the MySQL connections inside the back-end servers. This part is important, as it will synchronize all your data accross your spigot servers.
<br>

## Connecting to MySQL
As mentionned above, a MySQL database is needed to sync Ultra Scoreboards accross servers. To start your syncing process, connect to your server in-game, and open the plugin's GUI by executing the command `/uboards` in chat.
<br>

Then click on the Hook to extend the gui and see more options.
<br>

Then click on the Command Block in the bottom-left of the GUI. *(Called `Settings`)*
<br>

Then click on the EnderChest in the top-middle-right of the GUI. *(Called `MySQL Database`)*
<br>

Then click on the Emerald Block in the middle of the GUI. *(Called `Setup MySQL`)*
<br>

Then click on the Paper in the middle-left of the GUI. *(Called `Credentials`)*
<br>

This will close the GUI and ask you to enter your database's credentials.

Here you will need to fill in the credentials *(info)* of your database. By typing them in the chat in this order:
<br>

- Database IP - Format: 0.0.0.0
- Database Port - Usually: 3306
- Database Name - Depends on what you named your database.
- Database Username - Used to connect to your database.
- Database Password - Used to connect to your database.
<br>

*Here's a shortend version of the proxy installation process:*
`/uboards >> Settings >> MySQL Database >> Setup MySQL >> Credentials`

Once you have filled in all the credentials, you can now test the connection by clicking on the Emerald Ore in the middle-right of the GUI and confirm it by clicking a second time on the same slot. If your database has not connected or the test takes too long, you have entered the wrong credentials.
<br>

Once you have successfully connected the plugin to your database, restart your server and the proxy so the connection can be established.
<br>

When you have repeated this process for all of your servers, your plugin is now proxy-ready.
<br>


### Manual MySQL Entry
If your proxy isn't connected you need to do it manually.
<br>First, we need the MySQL key from a connected server. This can be found in there *\SERVER_DIRECTORY\plugins\UltraScoreboards*. 
Here you need to copy the MySQL key, and paste it inside the config of the proxy (same directory as above).
<br>

**`NOTE:` This key can continue on a second line, so make sure to copy it all!**
<br>

### `TIPS:`
- *If you made an error while entering your credentials, you will have to clear them and re-enter them.*
- *After typing your database credentials for the first time, instead of copying and pasting the same strings again and again, you can press the arrow up key, to go back to the messages you send, and finding your credentials. This will make the installation process much faster and easier.*
- *Once you're done setting up the database, you can wait until you entered the credentials in all the spigot servers to restart them. This will avoid restarting your proxy multiple times.*
