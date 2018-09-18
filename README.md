# Playbook de instalação do Nginx.


# Utilização:
git clone `git@github.com:Fellipe26/Playbook-install-Nginx.git`
cd Playbook-install-Nginx
ansible-playbook -i /nginx/hosts main.yml -vvv

# Testes:
ansible churrops -m command -a "getent passwd nginusr"

ansible churrops -m command -a "rpm -qa epel-release git vim wget curl"

ansible churrops -m command -a "systemctl status nginx"
