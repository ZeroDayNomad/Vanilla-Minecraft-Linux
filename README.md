# Vanilla-Minecraft-Server-May2022 (JAVA Edition)
Ansible Script to launch your own Minecraft Server for your friends.
<img src=https://almalinux.org/static/images/logo.svg>
<img src=https://www.letstechup.com/wp-content/uploads/2021/10/Minecraft-founder.jpg>

# Automation Script for Minecraft Servers - Vanilla Linux Script for AlmaLinux

This project is ongoing and will continue to be updated over time.
- Server Version 1.14

# Generating a Hashed Password For This Script:
```
sudo dnf -y install epel-release
```
```
sudo dnf install python3
```
```
python3 -c 'import crypt,getpass;pw=getpass.getpass();print(crypt.crypt(pw) if (pw==getpass.getpass("Confirm: ")) else exit())'
```
**It will immediately ask you to type in a password and then confirm it (Like The Example Below)**
```
Password: 
Confirm: 
$6$/1OFlW9yH1KHHiOm$pn2SfNgbF/rbblahjseab/p1Xb6Z29UZik.BUilZ.TLnp9yvl2HViB3fs8XdVteboeioss7o2A4g1IYxw.TFJ/
```
# Discord Webhooks:
In order to send Discord Notifications from Ansible, you will need to install the community add-on using:
```
ansible-galaxy collection install community.general
```
**Making a Webhook:**
Open your Server Settings and head into the Integrations tab:
Click the "Create Webhook" button to create a new webhook!
<img src=https://support.discord.com/hc/article_attachments/1500000463501/Screen_Shot_2020-12-15_at_4.41.53_PM.png>
You'll have a few options here. You can:

Edit the avatar: By clicking the avatar next to the Name in the top left

Choose what channel the Webhook posts to: By selecting the desired text channel in the  dropdown menu.

Name your Webhook: Good for distinguishing multiple webhooks for multiple different services.

You now have your own handy URL / pneumatic tube schoomp-er that you can link to more websites to receive messages from. 
<img src=https://support.discord.com/hc/article_attachments/360101553853/Screen_Shot_2020-12-15_at_4.51.38_PM.png>

# Update Log:
- 04/30/22: **Base Script Created, Fixed some errors**
