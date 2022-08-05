## Part 1. Установка ОС

Ubuntu version:
![Ubuntu_version](screenshots/Ubuntu_version.png)

---

## Part 2. Создание пользователя

* Creation of a new user:

![Create_new_user](Screenshots/new_user.png)

* cat /etc/passwd:

![Create_new_user](Screenshots/cat%3Aetc%3Apasswd.png)


## Part 3. Настройка сети ОС

* Для изменения имени машины редактируем файл, находящийся по этому пути: 
```
/etc/hostname
```

![Change_hostname](Screenshots/change_hostname.png)

* Меняем часовой пояс через команду ```timedatectl```

![Zone_location](Screenshots/timedatectl.png)

* Команда ```ip link show``` поможет вывести названия всех сетевых интерфейсов

![Network_interfaces](Screenshots/network%20interfaces.png)

_lo (loopback device) – виртуальный интерфейс, присутствующий по умолчанию в любом Linux. Он используется для отладки сетевых программ и запуска серверных приложений на локальной машине. С этим интерфейсом всегда связан адрес 127.0.0.1. У него есть dns-имя – localhost. Посмотреть привязку можно в файле /etc/hosts._


* IP-адрес, получаемый от DHCP:


![IP-address from DHCP](Screenshots/ip_address_from_dhcp.png)

__DHCP__  _(англ. Dynamic Host Configuration Protocol — протокол динамической настройки узла) — прикладной протокол, позволяющий сетевым устройствам автоматически получать IP-адрес и другие параметры, необходимые для работы в сети TCP/IP._

* Внутренний IP-адрес шлюза, он же IP-адрес по умолчанию:

![IP-address](Screenshots/local_ip-address.png)


* Внешний IP-адрес:
  
![IP-address](Screenshots/ip-address.png)


* Статический IP-адрес и DNS назначаем через config-файл ```netplan```

![Static IP](Screenshots/static_IP%2BDNS.png)


* Пингуется __"ВО"__!

![Ping](Screenshots/ping.png)