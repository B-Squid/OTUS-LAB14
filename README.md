# OTUS-LAB-14
<pre>
 Сбор и анализ логов
Не рекомендуется на машине с ELK уменьшать количество RAM, иначе некоторые сервисы на java могут просто не стартовать.

Для заполнения логов событиями можно использовать следующие команды:
curl http://localhost
curl http://localhost/dfgdfg
nginx -s reload (для наполнения /var/log/nginx/error.log)

Для того, что бы добраться до интерфейса kibana необходимо пробросить локальный порт в вагранте (например 5601 -> 56010)
 и потом сделать ssh-туннель (спасибо Владимиру Дроздецкому за открытый урок по ssh ;) например командой 
ssh -f -N -L 50000:127.0.0.1:56010 synergy@35.202.115.134 
После чего кибану можно откртыть в браузере локальной машины открыв ссылку вида http://127.0.0.1:50000
</pre>
