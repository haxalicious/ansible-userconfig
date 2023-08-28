# ansible-userconfig
Ansible role for initial user setup.
## Role variables
 - `ssh_key`:
   - Default: '~/.ssh/id_rsa.pub'
   - Description: Path to SSH public key.
 - `dotfiles`:
   - Default: ~/.dotfiles
   - Description: Path to dotfiles.
 - `shelluser`:
   - Default: '{{ ansible_user }}'
   - Description: User to install config for.