###ss
список сокетов `ss` - открытые сетевые подключения,  
какие IP адреса используются или какие порты прослушиваются

```sudo ss -tap | grep mysql```  
```sudo ss -tlap | grep mysql```  
`sudo ss -tr`  
`-t` - tcp, `-r` - resolve hostname