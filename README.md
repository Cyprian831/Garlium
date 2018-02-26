# My Garlium is broken!

This page should help with almost every issue with garlium once its installed, always feel free to message @Cyprian#2167 if something is not working or if you have any suggestions!

## Connection Issues

(Original fix found by @VeriFone#0710)

Connection issues with Garlium? This is likely because the nodes you currently have are overloaded. Adding more nodes seems to be the solution.

To add more nodes, shutdown Garlium, press `Win+R > %appdata%/Garlium` on windows and press `shift-command-g` to go to folder then its under `~/.garlium` for linux and mac and open `recent_servers` in a text editor, and replace what you have with :  
```
``[  
    "clovemines.fun:50002:s",  
    "172.93.54.31:50002:s",  
    "ske.wtf:50004:s",  
    "mhamburger.net:50002:s",  
    "garlium.kenzierocks.me:50002:s",  
    "electrum.garlicsoup.xyz:50002:s",  
    "electrum.grlc-bakery.fun:50002:s",  
    "garlium.grlc-bakery.fun:50002:s",  
    "electrum.garli.co.in:50002:s",  
    "garlium.garli.co.in:50002:s",
    "garlium.rshaw.space:50002:s",
    "garlium.garlicpool.org:50002:s",
    "roflmining.com:50002:s",
    "tuxprint.com:50002:s"
]``
```
Save, and start Garlium.
 
## If above doesn't work

-Under the tools option on the top bar select network

-In the new window select the server tab on the top

-Uncheck the box that says select server automatically

-In the server box input one of the servers below and the port in the adjescent box

-Click on close and wait a couple minutes for it to update

-If this doesnt work, repeat with a different serer

-If youve tried all the servers and its still not working recheck the box and restart the wallet client

Pools are at the bottom of this page:https://xske.github.io/garlium/

### Possible redo of above, awaiting response.

In Garlium, go to ` ``Tools>Network>Server`` ` Uncheck "Select Server Automatically"
Grab one of the listed servers (I Suggest `electrum.garlicsoup.xyz 50002`) and insert it in the `Server:` Box.
Click close and restart Garlium, then wait 2~ minutes. If failed, repeat with another server. If none of these work
check the "Select Servers Automatically" box and restart Garlium.

## Losing all post-fork coins

Go to "tools>network" and make sure youre in the "overview" tab. In the box there should be two dropdown menus, probably already open. Right click on the dropdown that has a higher "height" at the right of it and select "Follow this branch"

You should start recieving any garlic you lost right away!

## For "Server is Lagging" or "the transaction was rejected by network rules.\n\n64: Rejected/non-final"
 
Press `Win + R` and enter %appdata%/Garlium and delete ` ``blockchain_headers`` `
 
## For people who are asking why their address changed in their receive tab
 
Your old address is still there. Go to ` ``View -> Show addresses`` `
The switching thing is for anonymity on the receive tab
Cause you can use the QR code to make invoices essentially

## For Garlium if people are missing their coins or some extra are sent in a transaction
 
Go to `view > Show Coins`
and `view> Show Addresses`
In addresses, on the top left go to "Receiving" and change it to "Change"

## Absurdly high fees

Getting an absurdly high fees error? Try going to "View -> Show Coins". Every "coin" you see there is a UTXO. Select as many as you need to send by selecting the first one, holding "shift" and tapping "PG DN" (page down) on your keyboard to select about 20 at a time (don't select more than about 250, though), right click, and press "Spend". Now, select how much you want to spend, and send your money either to yourself (to "merge" UTXOs), or to someone else (they'll receive them as a normal transaction).

If consolidating wont work, try navigating to ` ``tools>preferences>transactions`` ` and deselect ` ``spend only confirmed coins`` `.

## Breadbox/GarlicoinWallet Coin Issue.

Regarding Breadbox/GarlicoinWallet: The way their Web-Wallets works is they have one large wallet that you
and many others using the wallet have access to. Because of this, the Receive address that
you use is not going to tell you accurately what is happening to your wallet.
This includes random outgoing transactions.
You will have to check your wallet manually in Breadbox/GarlicWallet if you want to have an accurate

## Failed to execute script garlium

Garlium may be corrupted, just redownload the exe and run again to fix this.

If redownloading doesn't work, try to delete everything in your garlium directory except for your wallet.dat and install fresh

## I can only connect to one node
Thanks to @Azlehria#2279 on discord for figuring this out!

Press "win+R" and enter ` ``%APPDATA%\Garlium\certs`` `. Once in the certs folder  Rename every file to remove the ".temp" extension from the end of every file.

###### [Take me back to the hub!](https://cyprian831.github.io/Garlicoin/)
