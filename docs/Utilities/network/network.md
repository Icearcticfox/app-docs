#### Смотрит открытые порты сокеты
>ss -tlpn
#### Смотрим свои сетевые интерфейсы
>ip a

>ip -route
#### NetCat
https://habr.com/ru/post/336596/

Проверка наличия открытого TCP-порта 12345
>nc -vn 192.168.1.100 12345

Сканирование TCP-портов с помощью netcat
>$ nc -vnz 192.168.1.100 20-24


### NetMap
Find All Hosts on Network
>nmap -sP 192.168.1.0/24 
> 
>nmap -sn 192.168.1.0/24



### ifconfig

- up - включить интерфейс;
- down - выключить интерфейс;
- (-)arp - включить или выключить использование протокола ARP для интерфейса;
- (-)promisc - включить или выключить неразборчивый режим для интерфейса;
- (-)allmulti - включить или выключить режим multicast;
- metric - изменить параметр metric;
- mtu - изменить максимальный размер пакета;
- netmask - установить маску сети;
- add - добавить ip адрес для интерфейса;
- del - удалить ip адрес интерфейса;
- media - установить тип внешнего протокола;
- [-]broadcast - установить широковещательный адрес или отключить эту функцию;
- hw - установить MAC адрес для интерфейса;
- txqueuelen - размер очереди интерфейса;

### [How to set hostname](https://linuxconfig.org/how-to-change-hostname-on-linux)
`/etc/hostname`
`sudo hostnamectl set-hostname linuxconfig`