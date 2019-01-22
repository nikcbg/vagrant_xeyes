# vagrant_xeyes

### Purpose of the repository 
- The purpose of the repository is to run an app on a Vagrant VM with graphical interface. 

#### List of files in the repository

File name                            | File description 
------------------------------------ | --------------------------------------------------------------
`scripts/provision.sh` | script that install x11 app that allows to run applications with graphical 
`.gitignore` | which files and directories to ignore in the repository.
`Vagrantfile` | file with sript that imports Vagrant box and installs script from `provision.sh` file.

### How to use this repository. 
- Install `Vagrant` by following this [instructions](https://www.vagrantup.com/downloads.html).
- Clone the repository to your local computer: `git clone git@github.com:nikcbg/vagrant_xeyes`.
- Go to the cloned repo on your computer: `cd vagrant_xeyes`.

### How to use the repository 

- check if x11 app accepts connections by executing:
``` xhost +```

- check if the local environment works by executing:
```
xeyes
```

- next create and configure your Vagrant machine by executing:
```
vagrant up
```

- finally login to the Vagrant box to run the graphical interface:
```
vagrant ssh -c 'xeyes`
```

### TO DO: 
- Check if everything works as expected. 
