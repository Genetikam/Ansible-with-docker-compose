# Ansible-with-docker-compose

# Используемый дистрибутив linux:
Ubuntu 22.04 LTS (Jammy Jellyfish).

# Инструкция:
'''
1) Устанавливаем ansible 2.10.8 любым удобным способом. Например, apt install ansible.
  
2) Генерируем ssh ключ root'а и копируем на хост, где будем устанавливать приложение.

3) Заменяем ip адрес в файле hosts на нужный нам и запускаем ansible-playbook Main.yml
'''
