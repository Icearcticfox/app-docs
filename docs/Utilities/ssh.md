#### Копируем ssh ключик на хост
> ssh-copy-id -i ~/.ssh/id_rsa.pub YOUR_USER_NAME@IP_ADDRESS_OF_THE_SERVER

```#!/bin/bash
for ip in `cat /home/list_of_servers`; do
    ssh-copy-id -i ~/.ssh/id_rsa.pub $ip
done
```

blowfish ускоряет копирование
>scp -c blowfish root@host:/home/itsecforu/* /home/itsecforu
### [Вопросы по ssh](https://itsecforu.ru/2022/01/10/%F0%9F%96%A7-30-%D0%B2%D0%BE%D0%BF%D1%80%D0%BE%D1%81%D0%BE%D0%B2-%D0%B8-%D0%BE%D1%82%D0%B2%D0%B5%D1%82%D0%BE%D0%B2-%D0%BD%D0%B0-%D0%B8%D0%BD%D1%82%D0%B5%D1%80%D0%B2%D1%8C%D1%8E-%D0%BF%D0%BE-ssh/)

Цикл выполнения команд для каждого хоста из файла
`for HOST in "cat hosts.txt"; do ssh -f "uptime; df -h" $HOST; done`

### Копирование на хост или с хоста
> scp [other options] [source username@IP]:/[directory and file name] [destination username@IP]:/[destination directory]