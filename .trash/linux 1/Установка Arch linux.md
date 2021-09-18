Здесь храняться полезные команды и кратки обьяснения для комфортной установки и настройки arch linux 

pacman -S wget 
wget matmoul.github.io/archfi - GUI программа для комфортной установки linux
sh archfi - запуск 
useradd -mg users -g wheel -s /bin/bash имя - добавление юзера и добавление его в группы users и wheel 
passwd имя - установка обьяз* пароля для пользователя 
pacman -Syu - установка базы сыллок и обновление всех зависимостей
pacman -S sudo - программа для запуска программ от root (нужна нстройка)
nano etc/sudoers - конфиг sudo ( в нем нужно стереть # для группы wheel)
nano etc/pacman.conf - конфиг pacman (При использовании multilub нужно отредактировать)
pacman -S xorg xorg-server xorg-aps - сервер x (GUI оболочка linux) также поначалу использует встроенный драйвер, но для лучшей работы нужны драйвера --> https://wiki.archlinux.org/index.php/xorg

pacman -S plasma-meta kde-applications - скачивание и установка KDE и приложений KDE

systemctl enable NetworkManager - демон программы NetworkManager для настройки internet

systemctl enable sddm - программа для автостарта сервера x
pacman -S base-devel - пакет для нормальной работы makepkg -sri 

pacman -S chromium - Google chrome 

pacman -S discord

[[Основа]][[обучение]][[Термины]][[Inbox/Study/Programs/linux 1/linux]]