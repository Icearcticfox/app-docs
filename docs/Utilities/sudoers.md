### Добавить юзеру права выполнять sudo без пароля

Добавление юзера в группу /etc/sudoers

`username  ALL=(ALL) NOPASSWD:ALL`

`echo "username  ALL=(ALL) NOPASSWD:ALL" | sudo tee /etc/sudoers.d/username`
>https://linuxize.com/post/how-to-add-user-to-sudoers-in-ubuntu/

