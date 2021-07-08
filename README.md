# Asus_Battery_Charge_Limiter
This is just to make the process automatic for the amazing python script made by cforrester1988. By following the below steps you can limit your battery thresold to your desired percentage value like 10--20--30--90% as per your need for asus laptops. I am not sure about other laptop brands.
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
