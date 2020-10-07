# psi

This is repository of heat templates to be used for PNTAE-Training courses in openstack cloud (like e.g. PSI)

## PREREQUSITE

- openstack cli must be pre-installed on theystem

  - RHEL
```
$ sudo yum -y install python2-openstackclient openstack-heat-api
```

  - Fedora
```
$ sudo yum -y install python3-pip 
$ sudo pip install openstacksdk
$ sudo pip install python-openstackclient python-heatclient
```

## HOW TO USE

- Clone this repo in user's HOME directory
```
$ git clone https://github.com/pntae-training/psi.git
```

- Create ~/rcfiles directory and then switch to ~/psi directory
```
$ mkdir ~/rcfiles/
$ cd psi/
```

- Copy psirc.sample file in psi directory to ~/rcfiles firectory
```
$  cp psirc.sample ~/rcfiles/
```

- Add your openstack login credentials to psirc file
```
$ grep KRB ~/rcfiles/psirc
export OS_USERNAME=KRBUSER
export OS_PASSWORD=KRBPASSWD
```

- Tweak .novelloshell.cfg file if you are not using recommended paths in these steps

- Finally run novelloshell-v4.sh script in psi directory to start using NovelloShell
```
$ ./novelloshell-v4.sh
```

#### NovelloShell: https://github.com/ashish-k-s/NovelloShell

