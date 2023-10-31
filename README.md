# Ansible-with-docker-compose

# Используемый дистрибутив linux:
Ubuntu 22.04 LTS (Jammy Jellyfish).
https://old-releases.ubuntu.com/releases/22.04/ubuntu-22.04-live-server-amd64.iso

# Инструкция:
1) Устанавливаем ansible 2.10.8 любым удобным способом. Например:
```
apt install ansible.
```  
2) Генерируем ssh ключ root'а и копируем на хост, где будем устанавливать приложение.
```
ssh-keygen && cat /root/.ssh/id_rsa.pub
```
3) Заменяем ip адрес в файле hosts на нужный нам и запускаем наш playbook.
```
ansible-playbook Main.yml
```
4) Проверяем работу приложения.
```
curl $server_ip:8080
```
