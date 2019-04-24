# custom-debian-script

As root : 

cd /root

git clone https://github.com/agencetca/custom-debian-script.git

cd custom-debian-script

chmod +x tca-install

./tca-install

[wait...]

When script has terminated, a user name is asked and the directory is changed to this user's home

As user :

  cd ~/.installation
  
  ./tca-install [windows] //if the keyword windows is provided, WinAte will be installed
  
[wait...]

At the end the computer reboots.

- Add links to panel at the bottom of the page.
- Configure printer (need to plug it in).
- Configure Skype.
- Configure Dropbox.
- Configure Recoll : files to index
- OR install searchmonkey : https://sourceforge.net/projects/searchmonkey/files/latest/download
- Add adblock for chromium.
- Add adblock for firefox.
- Modify Gedit Preferences > Fonts & Colors > Change colorscheme (otherwise selection lacks visibility)
- Modify Nautilus Preferences to Detailed View
- Open Chromium, right click on upper bar, select : Use system title bar and border

##### Mouse speed:
xinput --list --short
select the id of the device
xinput --list-props id_device
look the code number between the parenthesis ()
example : libinput Accel Speed (286):	0
          xinput --set-prop 12 286 1 (1=activated, 0=deactivated)
          #12 is the example id_device

