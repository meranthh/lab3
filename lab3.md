# Лабораторная работа №3
Открываем витуал бокс:

создаем 3 машины (A,В,С)

в настройках А в разделе сети ставим 3 адаптера(1 - сетевой мост, 2 - внутренняя сеть, 3 - внутренняя сеть)

в настройках B в разделе сети ставим 1 адаптера(1 - внутренняя сеть)

в настройках C в разделе сети ставим 1 адаптера(1 - внутренняя сеть)

дальше запускаем наши 3 ВМ и чкачиваем на них ubuntu

логинемся в каждой ВМ 

заходим в каждой ВМ и выполняем слудующие действия:

зайти в А и написать ping www.google.com (делаем скриншот)

пишем ip a (делаем скриншот где все пусто)

пишем sudo ip addr add 255.255.0.1/24 dev enp0s8

пишем ip a (делаем скрин того что у нас добавился ip в enp0s8)

заходим в B пишем пишем ip a (делаем скриншот где все пусто)

пишем sudo ip addr add 255.255.0.2/24 dev enp0s3

пишем ip a (делаем скрин того что у нас добавился ip в enp0s3)

заходим в А пишем ping 255.255.0.2 (делаем скрин что пакеты пошли)

далее в А пишем sudo ip addr add 255.255.1.1/24 dev enp0s9

пишем ip a (делаем скрин того что у нас добавился ip в enp0s9)

заходим в C пишем пишем ip a (делаем скриншот где все пусто)

пишем в С sudo ip addr add 255.255.1.2/24 dev enp0s3

пишем ip a (делаем скрин того что у нас добавился ip в enp0s3)

заходим в А пишем ping 255.255.1.2 (делаем скрин что пакеты НЕ пошли)

заходим в B пишем ping 255.255.1.2 (делаем скриншот что пакеты не идут)

заходим в С пишем ping 255.255.0.2 (делаем скриншот что пакеты не идут)

что бы выйти из ping надо нажать ctrl+C



![Screenshot_1](https://github.com/user-attachments/assets/5259cb85-5a44-40c0-bec3-b58f9288b801)

![Screenshot_2](https://github.com/user-attachments/assets/b1f7458e-8756-4f6e-b0d4-3bca140e6bb2)

![Screenshot_3](https://github.com/user-attachments/assets/6a1c3cdc-2539-426a-b5db-d0a88d847c49)

![Screenshot_4](https://github.com/user-attachments/assets/59ed70ca-e907-4a10-b4c3-34737c55ea2d)

![Screenshot_5](https://github.com/user-attachments/assets/f4ea104a-8606-48d6-8952-a305bb2ef6e2)

![Screenshot_6](https://github.com/user-attachments/assets/5bb4a5ef-1396-4624-9106-b1ff930aafdc)

![Screenshot_7](https://github.com/user-attachments/assets/5789ab5b-4177-48d6-8d29-16746718bc57)

![Screenshot_8](https://github.com/user-attachments/assets/f4e775ea-9d0b-46a8-bf0a-d33f6d8ad0db)

![Screenshot_9](https://github.com/user-attachments/assets/3223d592-fbc4-4037-bbe7-83a90b4c81af)

