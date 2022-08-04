# vagrant-ansible for Debian 9
VM with apache2:8888 &amp;&amp; nginx:80

Using the Vagrantfile, the VM is deployed with the following parameters:
CPU - 2 / RAM - 2 GB / HDD - 10 GB () / OS - Debian 9
###########################################################################

(the minimum disk size created was 20 GB, I assume that it depends on the image box, I also found information that the config.disksize.size plugin allows you to create at least 10 GB)

###########################################################################

Using ansible_local (playbook.yml) the following actions are performed:
 installing: 
             - vim +
 
             - wget +
             
             - htop +
             
             - tmux +
             
             - php5.6 - (there is no repository, after adding repository it gives a 403 error)
             
             - apache2:8888 +
             
             - nginx:80 +
             
helloworld.php - php file with text "Hello World!"
