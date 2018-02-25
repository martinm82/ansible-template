# ansible-template

An Ansible template showing all kind of Ansible features. This project is meant to be a reference
of all things I learned in Ansible and to use as well in upcoming Ansible projects.

## SSH user

* Create a SSH key-pair

```bash
$ ssh-keygen
```

* Store the private key in the *ssh_keys* folder with 0600 permissions
* Store the public key on remote in ~/.ssh/authorized_keys

```bash
$ cat ~/.ssh/id_rsa.pub > ~/.ssh/authorized_keys
```

* Add remote user to sudoers

```bash
$ echo "ansible ALL=(ALL) NOPASSWD:ALL" > /etc/sudoers.d/ansible
```
