# Django Twitter Api Template
If you don't use Pycharm then no need to gitignore .idea

### Vagrantfile.temp
- this file is just for show you content to copy and paste to the file just named 'Vagrantfile' with no file extension name
- once you paste the content to 'Vagrantfile', you can ignore this temp file, just remove it

### provision.sh:
- change your password
image skip tsinghua when oversea
- if first time you run `vagrant up` fail or half fail, try run `vagrant provision` to rerun the failed scripts

### Vagrant up fail classic error:
- `Command: ["hostonlyif", "create"]` with RED ERROR content
- [Solutions here](https://stackoverflow.com/questions/21069908/vboxmanage-error-failed-to-create-the-host-only-adapter)
- Mac specially happens due to system security
- First, in system privacy and security, under General Tab, unlock the icon with pw and allow VBox
- Then run the scripts in that link
- If all success without error prompt, you are good to rerun 'vagrant up'

### After Vagrant Up 'All Done!':
- use `vagrant ssh` to login server
- you can run python and import django and check version by django.VERSION
- after check, use `logout` to logout
