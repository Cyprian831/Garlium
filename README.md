## Connection Issues

(Original fix found by @VeriFone#0710)
Connection issues with Garlium? This is likely because the nodes you currently have are overloaded. Adding more nodes seems to be the solution.

To add more nodes, shutdown Garlium, press `Win+R > %appdata%/Garlium` and open `recent_servers` in a text editor, and replace what you have with :  
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
    "garlium.garlicpool.org:50002:s"
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

## For "Server is Lagging"
 
Press `Win + R` and enter %appdata%/Garlium and delete ` ``blockchain_headers`` `
 
## For people who are asking why their address changed in their receive tab
 
Your old address is still there. Go to ` ``View -> Show addresses`` `
The switching thing is for anonymity on the receive tab
Cause you can use the QR code to make invoices essentially

Removed small section because it is unconfirmed that un-checking that box will help.
## For Garlium if people are missing their coins or some extra are sent in a transaction
 
Go to `view > Show Coins`
and `view> Show Addresses`
In addresses, on the top left go to "Receiving" and change it to "Change"

## Absurdly high fees

Go to ` ``view > Show Coins`` `
Move to the coins tab
Select as many as you can with ''Ctrl click''
Right click and select ''spend''
Select the amount you desire and send it to an address of your own so that it can be sent more effeciently

Try going to View -> Show Coins. Every "coin" you see there is a UTXO. Select as many as you need to send (don't select more than about 250, though), right click, and press "Spend". Now, select how much you want to spend, and send your money either to yourself (to "merge" UTXOs), or to someone else (they'll receive them as a normal transaction).


## Breadbox/GarlicoinWallet Coin Issue.

Regarding Breadbox/GarlicoinWallet: The way their Web-Wallets works is they have one large wallet that you
and many others using the wallet have access to. Because of this, the Receive address that
you use is not going to tell you accurately what is happening to your wallet.
This includes random outgoing transactions.
You will have to check your wallet manually in Breadbox/GarlicWallet if you want to have an accurate

### Cyprians take at above ^

If you are losing coins randomly you might have originally used a breadbox wallet and since switched. 
You havent actually lost any coins, breadbox is just moving them around to a different address in your wallet. 
To recover these coins you will have to log on to your online wallet and transfer them out manually.

## Failed to execute script garlium

Garlium requires the windows binaries to work
You can download them right here: https://xske.github.io/garlium/
They are located just below the big "Installer for Windows" button

After you download this open it with 7zip or Winrar and extract the files inside.

If you've already done this and it doesn't work, then backup your wallet, save your key and seed, and reinstall

###### [Take me back to the hub!](https://cyprian831.github.io/Garlicoin/)
