# Linux troubleshooting

## Кейс: nginx не запускается
systemctl status nginx
journalctl -u nginx -xe

## Кейс: порт занят
ss -tulnp | grep :80
lsof -i :80

## Кейс: нет доступа к сайту
ping google.com
curl localhost

## Что делал
Диагностировал проблемы с сервисами, проверял логи, сеть и порты.

## Что понял
— как искать причину, если сервис не работает  
— как проверять сеть и доступность  
— как находить конфликты портов  
