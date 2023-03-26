### Структура

- Мониторинг
- Монтирование
- Регулярные выражения
- Системные процессы
- Иерархия директорий
- Загрузка Linux

#### Полезные команды  

запуск хром в фоновом режиме
`/Applications/Google\ Chrome.app/Contents/MacOS/Google\ Chrome --ignore-certificate-errors --ignore-urlfetcher-cert-requests &> /dev/null &`  
список запущенных приложений в фоновом режиме `jobs`

#### Просмотр журнала системы и / или сервисов
```journalctl```
```journalctl -u nginx```
https://logtail.com/tutorials/how-to-control-journald-with-journalctl/
