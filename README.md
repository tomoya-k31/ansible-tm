# ansible-tm


```sh
$ ansible-playbook -i hosts/osx osx.yml
```

## Requirements

- Ansibile 2.1
- Homebrew (for OSX)

## Setup for OSX

#### Install

- Install Xcode
- `$ sudo easy_install pip`
- `$ sudo pip install ansible --quiet`
- Install python library for faster compound processing

```sh
$ brew install openssl
$ env CRYPTOGRAPHY_OSX_NO_LINK_FLAGS=1 \
LDFLAGS="$(brew --prefix openssl)/lib" \
CFLAGS="-I$(brew --prefix openssl)/include" \
pip install cryptography
```

#### Upgrade Ansible
- `sudo pip install ansible --upgrade`
