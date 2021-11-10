WTF?
===

Сетапит на сервер wireguard, mtproto proxy в 
docker контейнер (`ansible-galaxy collection install community.docker`) и ставит nyancat в tty консоль.

# WG Key

Перед запуском генерим приватный и публичный ключи:

`wg genkey`

`echo $(wg genkey) | wg pubkey`

и записываем их в соответствующие vars в playbook.yml
