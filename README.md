# Asus_Battery_Charge_Limiter{Linux}
This is just to make the process automatic for the amazing python script made by [cforrester1988](https://github.com/cforrester1988). By following the below steps you can limit your battery thresold to your desired percentage value like 10--20--30--90% as per your need for asus laptops. I am not sure about other laptop brands.
#### To watch the original github repo here is the link:https://github.com/cforrester1988/asus-charge-control
## Step 1
Check if you can use this module or not by using the following command:\
<code>
lsmod | grep asus_nb_wmi\
</code>\
If you get something like:\
asus_nb_wmi 32768 0\
Then you are good to move forward.
## Step 2
Install python3 and pip3 also
#### for Ubuntu use following:
<code>
  sudo apt install python3 python3-pip
</code>

#### for Arch Linux use following:
<code>
  sudo pacman -S python3 python3-pip
</code>

#### for Solus OS use following:
<code>
  sudo eopkg install python3 python3-pip
</code>

## Step 3
Now let's install module:

<code>
  sudo pip3 install asus-charge-control
</code>

## Step 4
**a.** **Now download latest release [click here](https://github.com/ATinyLearner/Asus_Battery_Charge_Limiter/archive/refs/heads/main.zip)**\
After download extract the zip file and you will get 1 folder named **asus** and a file named **asuscharge70.service**\
**b.** Now open the extracted folder and copy asus folder to your home directory\
**c.** Now open the asuscharge70.service using any text editor and input ur user name in place of **your_user_name** then save the file and do the following:

<code>
sudo cp asuscharge70.service /etc/systemd/system/
</code>

## Step 5
Let's activate the service:

<code>
sudo systemctl enable asuscharge70.service
</code>

Now reboot your system and you are done. After Everyboot it will be set to 70%.\

# How to change battery percentage thresold?
Just open asus folder from your home directory and open asuscharge70.sh with any text editor and change 70 to your desired value and you are done.
