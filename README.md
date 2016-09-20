#Workspace for Ansible workshop

## Pre-reqs
- Python 2.6 or 2.7
- Ansible (which you can install via brew)

## Starting out
- Fork this repository
- Below are some sample tasks for practicing your Ansible skills
- To execute the ansible script, you can run ```ansible-playbook provisioning/site.yml```

## Tasks
- Install brew (if not installed already)
- Update homebrew
- Install with homebrew: vim
- Install with brew casks: atom, chrome, iterm2
- Install with shell: oh my zsh
- Create a role to install node using n (a node version manager, which you can get through homebrew)
  - The node role should use a variable to specify a particular version

## Sample Ansible task (for reference)

```
- name: Install package with yum
  yum: name=vim state=present update_cache=yes
  become: true
```

## Useful/relevant documentation
- [Intro to Ansible playbooks](http://docs.ansible.com/ansible/playbooks_intro.html)
- [Homebrew module](http://docs.ansible.com/ansible/homebrew_module.html)
- [Homebrew cask module](http://docs.ansible.com/ansible/homebrew_cask_module.html)
- [Shell module](http://docs.ansible.com/ansible/shell_module.html)

## Want to learn more?
- [Automating development environments with Ansible](http://www.nickhammond.com/automating-development-environment-ansible/)
