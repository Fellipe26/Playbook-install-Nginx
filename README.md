# Playbook de instalação do Nginx.

# Utilização:
git clone `git@github.com:Fellipe26/Playbook-install-nginx.git`
cd Playbook-install-nginx

ansible-playbook -i /nginx/hosts main.yml -vvv

# Teste:

ansible churrops -m command -a "getent passwd nginusr"

ansible churrops -m command -a "rpm -qa epel-release git vim wget curl"

ansible churrops -m command -a "systemctl status nginx"
