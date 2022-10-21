   13  sudo chown -R usera /mnt/data/ # à faire une seule fois
       pwd # `/home/usera/Bureau/sibpa_20-10-22-main/medias/vagrant_une_machine`

       # création de la machine
   14  vagrant up
   15  vagrant status
   16  vagrant ssh node1

       # connection à la machine en SSH directement
   21  vagrant ssh-config > ssh.config
   24  ssh -F ssh.config node1
       echo inventory # node1 ansible_ssh_common_args='-F ssh.config'


# installation ansible-lint 
python3.9 -m pip install ansible-lint