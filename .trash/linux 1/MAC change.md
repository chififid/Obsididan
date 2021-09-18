Смена MAC-адерса для Linux 

pacman -S macchanger  - программа для генерации и подмены mac-аддреса 

ip link - команда выводит все подключенные интерфейсы 

sudo ip link set dev 'interface' (example wlp3s0) down - выключить выбранный интерфейс
sudo ip link set dev 'interface' up -включить

sudo macchanger -e 'inteface'  -сгенерировать mac того же производителя, ключ -r генерирует совернно случ mac-адресс,
ключ -p ставит обратно заводской mac-аддрес 

sudo ip link set dev 'interface' address  XX:XX:XX:XX:XX:XX -изменить текущий mac-адресс y на XX:XX:XX:XX:XX:XX
[[Inbox/Study/Programs/linux 1/linux]]
