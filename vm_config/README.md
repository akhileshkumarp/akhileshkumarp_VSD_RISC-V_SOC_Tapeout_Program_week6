update default hostname to username to personal in the vm

[!default_hostname](./assets/default_hostname.png)

1. How to Change the Hostname
This is the name of your computer (e.g., what you see after the @ in your prompt: user@**hostname**). This is a safe and simple operation.

Set the new hostname: Replace new-hostname with your desired name.

Bash

sudo hostnamectl set-hostname new-hostname
Update the hosts file: This step is important to ensure sudo and other services continue to work correctly.

Bash

sudo nano /etc/hosts
You will see a file with lines like this:

127.0.0.1       localhost
127.0.1.1       old-hostname
Change old-hostname to match the new-hostname you just set. Save the file and exit (In nano, press Ctrl+O to save, then Ctrl+X to exit).

Apply changes: The change will be fully applied after you reboot your VM.

Bash

sudo reboot


[!updated_hostname](./assets/update_hostname.png)