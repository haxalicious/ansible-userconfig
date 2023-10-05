# ansible-userconfig
Ansible role for initial user setup.
## Role variables
 - `dotfiles`:
   - Default: ~/.dotfiles/dotfiles/
   - Description: Path to dotfiles.
 - `ssh_key_path`:
   - Default: ~/.ssh/id_rsa.pub
   - Description: Path to SSH public key.
 - `ssh_key`:
   - Default: Contents of `ssh_key_path`
   - Description: SSH public key.
 - `shell`:
   - Default: zsh
   - Description: Shell to install/use.
 - `shelluser`:
   - Default: '{{ ansible_user }}'
   - Description: User to install config for.
 - `privileged`:
   - Default: true
   - Description: Whether or not user has permissions to become another user. If false, disables all tasks that require root/sudo.
 - `pwauth`:
   - Default: 'no'
   - Description: Whether to allow SSH password authentication.
 - `rootlogin`:
   - Default: 'prohibit-password'
   - Description: Whether to allow root login over SSH.