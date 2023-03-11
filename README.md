## Installation 
* Activate a [Google Cloud Shell](https://console.cloud.google.com/) on Google cloud.
* Clone this GitHub Project into the Console:
```
git clone https://github.com/XongBong/terrariaserver
```
* Go into `terrariasrv` directory:
```
cd terrariasrv
```
* Allow all commands executable:
```
chmod +x *
```
* Run the Installation Script:
```
./install
```
Follow the installation step shown in the console
* Run the Start Server Script:
``` 
./startserver
```
## Joining your Server
* To join your server, start your server by doing `./startserver` *(If you haven't started it yet)* and do this command:
``` 
screen -r playit
```
- Now click the **Claim URL** and it should show you your host IP and Tunnel Server.
- Once your in that page, scroll down and click **Add Tunnel** on Minecraft Java/Bedrock and next to the **Local server address**, click **Add**.
- Now copy the generated dedicated IP something along with `auto.playit.gg` and copy it into the Server Address in Terraria and now you can play the server.

*(Note: If you want to change the Claim URL, you need to Stop the Server. This will reset your server IP.)*

## Accessing Server Console
* To access your server console, open this following session:
```
screen -r server
```
To completly stop the server, you can do `./stopserver` on the Linux console or do `exit` or `stop` on the Terraria console

## Detaching Screen/Session
* To Detach the session you can do it using the following keyboard shortcuts 
`CTRL + A` then press `D`

## Access Server Files
If you want to access your server files, go to `Open Editor` on the top right.
- Once you there, if you don't see any folders on the left side, you can `Open Folder` and pick `terrariasrv` and go to `terrariaserver` to view and modify anything inside.
- If you made any changes on your server, restart your server.
After you restarted your server, all the changes are saved into your server.

## Restarting your Server
If you don't know what restarting your server mean, here's the step.
- Go to `terrariasrv` or `../terrariasrv/` directory and do this command.
- Stop the server which stops both the Terraria Server and Playit.gg tunneling system:
```
./stopserver
```
- And now start your server again:
```
./startserver
```
Now your server has fully restarted.
## Keeping the Server Alive 24/7
There's only **ONE** way to keep your server online longer than 20 minutes:
- You must Keep your browser open to keep your server online. This so the shell doesn't get terminated when it's unused or the browser is closed.

*(Don't worry, your device that is being used to host your server isn't affected from the intensity of your server.)*

If you have any method the would possibly keep the server alive 24/7, feel free to **Fork** this project and request a **Pull** to this project. Any help will be greatly appreciated.

## Limitation of this project
### Google Cloud Shell Quota
While I was editing this project, I notice that Google has added a quota for each Cloud Shell uses and you can only host your server for the max of `50` hours per `Week`.
Once you used all of the hours, you can't use it again until next week.
### No Dedicated IP
Sadly you can't use the host IP into your dedicated IP as it won't let you join that server, you can only join your server by the generated dedicated IP provided by **playit.gg**. If you know how to reverse proxy the tunnel system, you *can* actually use the host IP to make a dedicated IP for your server but I highly doubt that would ever happen.
### Mixed Server Specs
Each Cloud Shell session will have different specs of your server based on your physical location so you won't always get the best performance of your server but good news being that it's always the range between `8GB` to `16GB` so you won't have to worry about lag when playing in the server with high processing in your server.

## Uninstall/Remove the Server
- If you want to make a new or delete your server, do this command inside `~/terrariasrv`:
```
./uninstall
```
It will tell you if you really want to uninstall it or not.

- This will remove the whole server folder and you can make a new one again by doing `./install`
## Deleting/Updating the whole Project
This project will constantly update day after day until I make a perfect project. If you have install this project before and it has some lack of features, you can update the project by doing this steps.
- First, go to the default folder
```
cd
``` 
- Now delete the whole project *(Be careful, backup/download your world folder FIRST before deleting it. You can't go back once you do this command)*:
```
sudo rm -r terrariasrv
```
If the project is completely deleted, you can [Clone the Project](https://github.com/XongBong/terrariaserver/blob/main/README.md#installation) again and it should be up to date with the new features and code from this project!
## Conclusion
Now you can host your very own Terraria Server fast and easy and it won't cost you a single penny to make a fast and strong server. Best of all, IT'S FOREVER! Feel free to leave any requests you would like me to add into the project. If you have any issues, go to the [**Issues**](https://github.com/XongBong/terrariaserver/issues) tab and submit a issue there.
## Credits
> Project Creator: *[XongBong](https://github.com/XongBong/)*
