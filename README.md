# ansible-userconfig
Ansible role for initial user setup.
## Role variables
 - `dotfiles`:
   - Default: ~/.dotfiles
   - Description: Path to dotfiles.
 - `ssh_key_path`:
   - Default: ~/.ssh/id_rsa.pub
   - Description: Path to SSH public key.
 - `ssh_key`:
   - Default: Contents of `ssh_key_path`
   - Description: SSH public key.
 - `shelluser`:
   - Default: '{{ ansible_user }}'
   - Description: User to install config for.
 - `pwauth`:
   - Default: 'no'
   - Description: Whether to allow SSH password authentication.
 - `rootlogin`:
   - Default: 'prohibit-password'
   - Description: Whether to allow root login over SSH.