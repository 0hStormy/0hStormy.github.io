# Creating Install Media

Creating install media is pretty easy, this section also assumes you're using Windows, as MacOS is its own rabbit hole and if you use Linux, you should know how to do this already.

You will need the following:

* Non-important USB Drive, 4gb or higher
* A computer
* An internet connection

<hr>

## Step 1: ISO File and Etcher

First, you'll need to download Etcher, which is a ISO writing tool, an ISO is a disk image that can written to DVD's or USB drives, which you can download at https://etcher.balena.io/.

Next you'll need to download the version of Fedora you chose, there are links to the ones I featured in the last section.

Now, open up Etcher, and you will see a Window that looks something like this:

<img src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2F4sysops.com%2Fwp-content%2Fuploads%2F2023%2F05%2FThe-BalenaEtcher-user-interface.png&f=1&nofb=1&ipt=0806d5aa8029bc2469e3e73df82bbac2f424355cf1a212038dd1cad3a1a4687b&ipo=images">

From here, click `Flash from File` and choose the ISO you download in your file picker. Then select the USB drive you want to write to with `Select Target`, **WARNING: Be very sure you clicked the correct drvie as it could wipe your OS or Data if you're not careful!** Finally, click `Flash!` to flash to USB drive with your ISO file of choice.

And if everything goes thorugh correctly, your USB should have Fedora on it now!