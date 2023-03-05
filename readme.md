# Ansible playbook to setup custom terminal

This is an ansible playbook to setup both zsh plugins and oh-my-posh custom terminal theme.

![image](https://user-images.githubusercontent.com/27609953/222961450-5bd1dc80-6173-42e4-bd50-b063ff3d3ae5.png)

The ansible playbook basically follows the 2 gists ([here](https://gist.github.com/Jason-CKY/476fcfc6970cd8553fa3b8552db5624e) and [here](https://gist.github.com/Jason-CKY/27d78f9c3fb663e9421b76026b0fbfb0)) I've written to:

* Install zsh
* Set zsh as default shell
* Install zsh plugins
* Install oh-my-posh
* Copy my custom theme

## Usage

Edit the `inventory` file to add your machines' IP addresses

```sh
ansible-galaxy role install -r ./requirements.yml
ansible-playbook -i ./inventory main.yml --ask-become-pass
```
