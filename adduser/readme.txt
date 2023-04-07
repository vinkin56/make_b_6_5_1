Порядок добавления пользователя и ключа:
Генерируем пару: 
ssh-keygen -f ~/.ssh/User1 -t rsa

Шифруем ключ:
ansible-vault encrypt --ask-vault-pass ~/.ssh/User1.pub

Запукаем ansible-playbook так:
ansible-playbook --ask-vault-pass sshtodo_b_651.yml
