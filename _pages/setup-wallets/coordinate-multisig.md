---
title: Coordinate Multisig
---

Now that we have all your public key information in Specter-Desktop, we need to create your `2-of-3` multisig wallet.
We tell Specter-Desktop and each hardware wallet that these are your 3 public keys and that any 2 of them is sufficient to sign a transaction.
This is a one-time setup that you'll never need to repeat.

## Configure Multisig Wallet in Specter-Desktop

1. On Specter Desktop, select `+ Add new wallet` > `Multisignature wallet` 
![](/assets/img/coordinate-multisig-specter-desktop-add-wallet.png){:width="85%" class="border_image"}

1. Give a name to your wallet (e.g. `Redundant Multisig`), choose `Segwit` (default), `2-of-3` (default) and select your 3 cosigners: `Keystone`, `Coldcard` and `Paper Wallet`
![](/assets/img/coordinate-multisig-specter-desktop-quorum.png){:width="85%" class="border_image"}
   
1. Select your public keys. If you've followed the default steps, you'll just select all 3 of them.  
![](/assets/img/coordinate-multisig-specter-desktop-keys-1.png){:width="85%" class="border_image"}
![](/assets/img/coordinate-multisig-specter-desktop-keys-2.png){:width="85%" class="border_image"}


1. See your first bitcoin address!   
![](/assets/img/verify-address-specter-desktop.png){:width="85%" class="border_image"} 
(we'll learn how to trustlessly verify addresses in the [Verify Receive Address section](/verify-receive-address/))

r multisig w
Now that we have our multisig wallet configured in Specter-Desktop, we need to let the Keystone and Coldcard devices know about it.

## Setup Keystone
1. On Specter-Desktop, select your multisig wallet (e.g. `Redundant Multisig`) > `Settings` > `Export` > `Show Keystone QR Code`:  
![](/assets/img/coordinate-multisig-specter-desktop-export-keystone.png){:width="85%" class="border_image"}

Specter-Desktop will display a popup like this:  
![](/assets/img/coordinate-multisig-specter-desktop-export-keystone-qr.png){:width="35%" class="border_image"}

1. Scan the QR code on your Keystone:  
![](/assets/img/coordinate-multisig-specter-desktop-import-keystone-qr.png){:width="85%" class="border_image"}
   
1. View wallet information and confirm:    
![](/assets/img/coordinate-multisig-specter-desktop-keystone-imported.png){:width="25%" class="border_image"}
![](/assets/img/coordinate-multisig-view-policy-onsetup-keystone.png){:width="25%" class="border_image"}

## Setup Coldcard
1. On Specter-Desktop, select your multisig wallet (e.g. `Redundant Multisig`) > `Settings` > `Export` > `Download Coldcard File`:  
![](/assets/img/coordinate-multisig-specter-desktop-export-coldcard.png){:width="85%" class="border_image"}

1. Save this file to your microSD card and put the microSD card in your Coldcard.  

1. On your Coldcard, go to: `Settings` > `Multisig Wallets` > `Import from SD`  
![](/assets/img/coordinate-multisig-coldcard-create-airgapped.png){:width="85%" class="border_image"} 
(select the file and press "OK" (???))


{% include next_steps.md next_url="/verify-receive-address" next_name="Verify Receive Address" %}
