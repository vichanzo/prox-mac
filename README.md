# prox-mac
Notes on my second attempt.  Use this on your own risk - I am using this to document my process.

## Steps
1) Install from Debian 12 netinstaller using Easy2boot
   - partition with 300 GB extra partition (save for LVM)?
   - rest was guided partitioning
2) Install the pre-reqs for Ansible
   - apt install git sudo openssh-server ansible  
3) Create ssh keys and add to Github Repo
   ssh-keygen
4) Clone the repo
   - git clone https://github.com/vichanzo/prox-mac
   - git clone git@github.com:vichanzo/prox-mac
5) cd prox-mac
6) Run the playbook
   - ansible-playbook local.yml
   - playbook will - install basics (neofetch htop tmux)
   - install xfce4
   - 
