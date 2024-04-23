# Сеть 101
> ⚠ Сеть 101 представляет из себя простое введение в наиболее важные сетевые концепты этического хакинга. В целом это огромная тема и я рекомендую покурить различные источники по типу спецализированных курсов, книг, и сертификатов по типу [Cisco CCNA](https://www.cisco.com/c/en/us/training-events/training-certifications/certifications/associate/ccna.html) или [CompTIA Network+](https://www.comptia.org/certifications/network). Кстати, тут вы можете найти кучу **бесплатного тернинга**, который я бы рекомендовал вам [посмотреть](https://freetraining.dfirdiva.com/free-networking-training) позднее.

### Цели
* Понимание базовых сетевых концептов 

### **Этот модуль придерживается следующего порядка:**
1. [Введение](/0-Core-Knowledge/0-Networking-101.md#1-введение)
2. [IP и MAC адреса](/0-Core-Knowledge/0-Networking-101.md#2-ip-и-mac-адреса)
3. [Подсеть](/0-Core-Knowledge/0-Networking-101.md#3-подсеть)
4. [TCP/UDP и Трехстороннее рукопожатие](/0-Core-Knowledge/0-Networking-101.md#4-tcpudp-и-трехстороннее-рукопожатие)
5. [Порты & Протоколы](/0-Core-Knowledge/0-Networking-101.md#5-порты--протоколы)
6. [Модель OSI](/0-Core-Knowledge/0-Networking-101.md#6-модель-osi)

# 1. Введение

## Да что, чёрт побери, такое эта ваша Сеть?
Если в кратце, сеть состоит из 2х или более компьютеров, которые соединены, чтобы обмениваться данными. Компьютерные сети это базис коммуникации в IT. Они могут использоваться огромным количеством способов и могут включать много различных типов сетей. Компьютерная сеть это набор комьютеров, соединённых вместе так, что они могут обмениваться информацией. наиболее ранние экземпляры компьютерных сетей датируются 1960ми, но за следующие пол столетия они прошли огромный путь развития.

![net](https://gist.githubusercontent.com/Samsar4/62886aac358c3d484a0ec17e8eb11266/raw/5edc8fbef915a17c93fa91c95877134c8fac324c/net2.jpg)

<sub><sup>Сетевая топология LAN - SOHO / Small Office Home Office</sup></sub>

**Два самых распространённых типа сетей называются LAN (Local Area Network) и WAN (Wide Area Network)**

## Топологии
Существое много различных типов сетей, которые могут использоваться для различных целей разными людьми и организациями. Вот некоторые типы сетей с которыми вы можете столкнуться:

### LAN - Local Area Network - Локальная сеть

* LAN это сеть, которая имеет логические и физические границы, которые компьютер может передавать.

<p align="center">
<img width="70%" src="https://www.geocities.ws/alcantara97/starhttt.gif" />
</p>

### WAN - Wide Area Network - Глобальная сеть

* WAN это несколько LAN и/или дополнительных WAN сетей с функцией маршрутизации для обеспечения межсетевого взаимодействия.

<p align="center">
<img width="70%" src="https://gist.github.com/Samsar4/62886aac358c3d484a0ec17e8eb11266/raw/a3f9b5f3f243467208da83e0d0e543b32233c5d6/wan-topo.jpg" />
</p>

### MAN - Metropolitan Area Network - Муниципальная сеть

* MAN объединяет компьютеры в пределах города, представляет собой сеть, по размерам меньшую, чем WAN, но большую, чем LAN сети. Они предназначены для обслуживания территории крупного города — мегаполиса.

<p align="center">
<img width="70%" src="https://gist.githubusercontent.com/Samsar4/62886aac358c3d484a0ec17e8eb11266/raw/f37cec4e00f726cb4be3661f20ccad77751e003a/man-topo.jpg" />
</p>

### Интернет
Фактически огромное количество WAN сетей, соединённых между собой другими WAN сетями до тех пор, пока весь мир не стал Интернетом.

* Протокол, по которому работает Интернет, — TCP/IP.
  >Конечно, если вы используете законный адрес IPv4 или IPv6.
<p align="center">
<img width="70%" src="https://gist.githubusercontent.com/Samsar4/62886aac358c3d484a0ec17e8eb11266/raw/8c176b8a798fb5749c4391c45015ee5d14d56f13/internet.png" />
</p>

### Интранет
Если вы используете TCP/IP и делаете собственную LAN или WAN - вы создаёте Интранет.

* Проще говоря, Интранет это частная сеть, которая всё ещё использует TCP/IP

<p align="center">
<img width="70%" src="https://gist.githubusercontent.com/Samsar4/62886aac358c3d484a0ec17e8eb11266/raw/8c176b8a798fb5749c4391c45015ee5d14d56f13/intranet.png" />
</p>

## Обще-сетевая терминология
* **IP (Internet Protocol) адрес**: сетевой адрес системы в сети, который также известен как логический адрес.

* **MAC адрес**: MAC-адрес или физический адрес однозначно идентифицируют каждый хост. Он связан с сетевой интерфейсной картой (Network Interface Card - NIC).

* **Открытая система**: открытая система подключена к сети и подготовлена ​​к подключению.

* **Закрытая система**: закрытая система не подключена к сети, следовательно к ней невозможно подключиться.

* **Порт**: порт - это канал через который информация может быть получена и отправлена.

* **Узлы**: узл — это термин, используемый для обозначения любых вычислительных устройств, таких как компьютеры, которые отправляют и получают сетевые пакеты по сети.

* **Сетвые пакеты**: информация, которая принимается и отправляется по сети через узлы.

* **Роутеры**: Роутер (он же маршрутизатор) — это аппаратное оборудование, которое управляет пакетами. Он определяет, из какого узла пришла информация и куда ее отправить. Маршрутизатор имеет протокол маршрутизации, который определяет, как он взаимодействует с другими маршрутизаторами.

* **‍Преобразование сетевых адресов (‍Network address translation - NAT)**: метод, который маршрутизаторы используют для предоставления интернет-услуг большему количеству устройств с использованием меньшего количества общедоступных IP-адресов. Маршрутизатор имеет общедоступный IP-адрес, но устройствам, подключенным к нему, назначаются частные IP-адреса, которые не могут видеть другие люди за пределами конкретной сети.

* **Протокол динамической конфигурации хоста (Dynamic host configuration protocol - DHCP)**: назначает хостам динамические IP-адреса и поддерживается интернет-провайдером.

* **Интернет провайдеры (Internet service providers - ISP)**: компании, которые предоставляют интернет соединение, как обычным людям, так и другим компаниям/организациям.

# 2. IP и MAC адреса
## Что такое IP адрес (Internet Protocol)?
![ip](https://media.fs.com/images/community/upload/wangEditor/201912/24/_1577182449_2uLs0pQcuT.jpg)

IP адрес это уникальный адрес, который идентифицирует устройство в интернете или локальной сети. IP происходит от "Интернет Протокол", который обозначает набор правил, регулирующих формат данных отправляемых через интернет или локальную сеть.

## Проверяем свой локальный IP адрес

1. Если вы используете Linux или MacOS, то вам нужно открыть свой терминал и напечатать команду `ifconfig` 
2. Если вы используете Windows, то вам нужно отрыть командную строку, или powershell и напечатать команду `ipconfig /all`

![inet](https://gist.githubusercontent.com/Samsar4/62886aac358c3d484a0ec17e8eb11266/raw/5a56240010acbc33026413ad6b5c6f66e9450413/inet.png)

- inet IPv4: `192.168.64.3`
   - `inet` --> inet (Internet protocol family) показывает локальный IP адрес. Это IP 4ой версии (IPv4), использующий 32-битное десятичное число.
- inet6 IPv6: `fe80::c83b:ccff:fe0e:1069`
   - `inet6` --> Это IP 6ой версии (IPv6), использующий 128-битное шестнадцатеричное значение.
- `ether` --> MAC адрес - уникальный идентификатор присвоенный контроллеру сетевого интерфейса (network interface controller - NIC)

## Подробнее о десятичном значении IPv4:

``` 
IPv4 = диапазон 32 бита (4 октета по 8 бит, от 0 до 255 каждый)

11000000.10101000.01000000.00000011   [IPv4 двоичное значение]
   192  .   168  .   64   .  3        [IPv4 десятичное значение]
``` 

### Арифметика, стоящая за IPv4:

- В одном октете 8 бит:

0 или 1 | 0 или 1 | 0 или 1 | 0 или 1 | 0 или 1 | 0 или 1 | 0 или 1 | 0 или 1 
-|-|-|-|-|-|-|-
8ой бит | 7ой бит | 6ой бит | 5ой бит | 4ой бит | 3ий бит | 2ой бит | 1ый бит
128 (2^7) | 64 (2^6) | 32 (2^5) | 16 (2^4) | 8 (2^3) | 4 (2^2) | 2 (2^1) | 1 (2^0)

Вот как двоичные октеты преобразуются в десятичные: Самый правый или наименее значимый бит октета содержит значение 2^0. Бит слева от него содержит значение 2^1. Это продолжается до тех пор, пока не появится самый левый или самый значимый бит, который содержит значение 2^7. Итак, если все двоичные биты равны единице, десятичный эквивалент будет равен 255, как показано здесь:

```
  1   1   1   1   1   1   1   1
  |   |   |   |   |   |   |   |
(128 +64 +32 +16 +8  +4  +2  +1) --> 255 

Пример преобразования октетов:
IP Aадрес: 192.168.64.3


Чтобы вычислить первый октет (192.), из двоичного формата в десятичный:

128  64  32  16  8   4   2   1         
 |   |   |   |   |   |   |   |
 1   1   0   0   0   0   0   0          
 |   |   |   |   |   |   |   |
128+ 64+ 0+  0+  0+  0+  0+  0 = 192   ---> итоговое значение (первый октет IPv4 в десятичном формате)
```

* Возьмём следующий IP: `192.168.64.3`
* Первый октет `192` в 8-битном двоичном формате будет `1100 0000`.
* Включены только `8-й` и `7-й бит`, а остальные (биты с `6-го по 1-й`) выключены. Это означает, что десятичное значение представляет собой окончательную сумму этих значений: `128 + 64 = 192`

⚠️ **Почему? Компьютеры видят все в двоичном формате; включить и выключить.**


## IPv4 и IPv6
![ipv](https://academy.avast.com/hs-fs/hubfs/New_Avast_Academy/IPv4%20vs.%20IPv6%20What%E2%80%99s%20the%20Difference/IPv4-vs-IPv6.png?width=2750&name=IPv4-vs-IPv6.png)

## Частные and Публичные IP адреса
Все IPv4 адреса можно поделить на две основные группы: **глобальные (или публичные, внешние)** - эта группа также называется "WAN addresses" — те, что используются в интернете, и **частные (или локальные, внутренние) адреса** — те, что используются в локальной сети(LAN).

![priv-pub](https://wiki.teltonika-networks.com/wikibase/images/thumb/a/a7/Sip.png/1100px-Sip.png)

## Подробнее о **Частных IP** адресах:
Приватные (внутренние) адреса не маршрутизируются в интернете и на них не может быть отправлен трафик из интернета, они предполагались только для работы внутри локальной сети.
Частные адреса включают в себя IP адреса из следующих подсетей:

![private-ip](https://66.media.tumblr.com/02a533c1d55ca0ba83e0176168df06ec/tumblr_inline_o4m1taQugo1u4ytoo_1280.jpg)

## Преобразование сетевых адресов (‍Network address translation - NAT)
NAT stands for network address translation. It’s a way to map multiple local private addresses to a public one before transferring the information. Organizations that want multiple devices to employ a single IP address use NAT, as do most home routers. 

![nat2](https://gist.githubusercontent.com/Samsar4/62886aac358c3d484a0ec17e8eb11266/raw/8275f73b57bdcb982b1d69aa8d213d2bdb384657/nat2.png)

1. **Static NAT**

   When the local address is converted to a public one, this NAT chooses the same one. This means there will be a consistent public IP address associated with that router or NAT device.

2. **Dynamic NAT**

   Instead of choosing the same IP address every time, this NAT goes through a pool of public IP addresses. This results in the router or NAT device getting a different address each time the router translates the local address to a public address.

### ⚠️ IP Addresses operates on **Layer 3 of OSI Model**

*Note: This module will cover OSI model later.*

![osi3](https://gist.githubusercontent.com/Samsar4/62886aac358c3d484a0ec17e8eb11266/raw/b9d7f33be654d299f6618feeacb97fc5fd5bd7d2/OSI_L3.png)

# 3. Подсеть
### Why subnetting?
The way IP addresses are constructed makes it relatively simple for Internet routers to find the right network to route data into. However, in a Class A network (for instance), there could be millions of connected devices, and it could take some time for the data to find the right device. This is why subnetting comes in handy: subnetting narrows down the IP address to usage within a range of devices.

Because an IP address is limited to indicating the network and the device address, IP addresses cannot be used to indicate which subnet an IP packet should go to. Routers within a network use something called a subnet mask to sort data into subnetworks.

> ⚠️ Subnetting is really important for penetration testers and aspiring hackers, eventually you will face several cases involving small or large networks in your future engagements. Understanding the IP address type, range, available hosts is crucial for any network analysis.

## Cheat sheet makes easier for subnetting

![subnetting](https://gist.githubusercontent.com/Samsar4/62886aac358c3d484a0ec17e8eb11266/raw/5ce4b7daa9c2c10ccd44675eadaceae646e487e2/cyber-mentor-subnetting.png)

* CyberMentor Subnetting Sheet: https://twitter.com/thecybermentor/status/1211335431406727169

* Subnetting Cheat sheet alternative: https://nsrc.org/workshops/2009/summer/presentations/day3/subnetting.pdf



## Exercises:
Subnetting comes in handy to awnser basic questions like:
   - Identify the network and broadcast address
   - How many hosts available in the network/hosts range?
   - What masks allow the particular host?


IP range | Subnet | Hosts | Network | Broadcast
-|-|-|-|-
192.168.1.16/28 | 255.255.255.240 | 14 | 192.168.1.16 | 192.168.1.31 
192.168.0.0/22 | ? | ? | ? | ?

- Take the `192.168.0.0/22` IP range listed above
- You can easily figure out the subnet mask by look the cheat sheet, you can see the `252` column. Just replace the value of `x`. You will get `255.255.252.0`
   - Subnet masks can be 0, 128, 192, 224, 240, 248, 252, 254 and 255. 
   - To understand the basics of math behind the bits, check the next figure below:

![bits](https://gist.githubusercontent.com/Samsar4/62886aac358c3d484a0ec17e8eb11266/raw/c1e01e29aedc394f2d75c4ccf57e72606775103a/bits.png)

- The number of hosts is `2^(n) - 2`. 
   - `n = off bits`
   - In this case, is 2^10 = 1024 -> 1024 - 2 = `1022`
- The network portion is the first and lowest possible value.
- The broadcast is the last and highest possible value.

IP range | Subnet | Hosts | Network | Broadcast
-|-|-|-|-
192.168.0.0/22 | 255.255.252.0 | 1022 | 192.168.0.0 | 192.168.3.255



## Other relevant information about  IPs
- **IPv4 Main Address Types**
  - **Unicast** - acted on by a single recipient
  - **Multicast** - acted on by members of a specific group
  - **Broadcast** - acted on by everyone on the network
    - **Limited** - delivered to every system in the domain (255.255.255.255)
    - **Directed** - delivered to all devices on a subnet and use that broadcast address
- **Subnet mask** - determines how many address available on a specific subnet
  - Represented by three methods
    - **Decimal** - 255.240.0.0
    - **Binary** - 11111111.11110000.00000000.00000000
    - **CIDR** - x.x.x.x/12   (where x.x.x.x is an ip address on that range)
  - If all the bits in the host field are 1s, the address is the broadcast
  - If they are all 0s, it's the network address
  - Any other combination indicates an address in the range

# MAC Addresses 

-  MAC (Media Access Control) address is provided by NIC Card'd manufacturer and gives the physical address of a computer.

![macphys](https://i1.wp.com/learntomato.flashrouters.com/wp-content/uploads/MAC-address-hardware.jpg?resize=560%2C315&ssl=1)

The first three bytes of a MAC address were originally known as **OUI’s, or Organizational Unique Identifiers.  Each manufacturer of networking equipment was assigned an OUI, and was free to assign their own numbers in that block.**

```
   OUI     NIC
    |       |
________ ________
00:0c:29:99:98:ca
```
## Checking vendor behind MAC addresse
1. Check your MAC address use the command `ifconfig` (Linux) or `/ipconfig` (Windows)
![mac](https://gist.githubusercontent.com/Samsar4/62886aac358c3d484a0ec17e8eb11266/raw/214242916f8947f09fc15d5bdde6a668fd4a4c1f/mac2.png)

2. Copy and save the **first three bytes** of your address. *(The first three bytes from image above is `00:0c:29`)*

3. Validate the information by performing a **MAC Address Lookup** on the internet. For this example I'm using: https://aruljohn.com/
![mac2](https://gist.githubusercontent.com/Samsar4/62886aac358c3d484a0ec17e8eb11266/raw/c82686452d3e671f9a4d351cd5c02171914dd16d/mac2lookup.png)

4. As you can see the OUI lookup identify a virtual network interface provided by VMware 

*So, to summarize, the **first three bytes** are assigned to a manufacturer of networking equipment and the manufacturer assigns the last three bytes of an address.*

### ⚠️ MAC Addresses operates on Layer 2 of OSI Model
![osil2](https://gist.githubusercontent.com/Samsar4/62886aac358c3d484a0ec17e8eb11266/raw/b9d7f33be654d299f6618feeacb97fc5fd5bd7d2/OSI_L2.png)

# 4. TCP/UDP и Трехстороннее рукопожатие

## Transmission Control Protocol/Internet Protocol (TCP/IP)

* What is TCP used for?

TCP enables data to be transferred between applications and devices on a network. It is designed to break down a message, such as an email, into packets of data to ensure the message reaches its destination successfully and as quickly as possible.

* What does TCP mean?

TCP means Transmission Control Protocol, which is a communications standard for delivering data and messages through networks. TCP is a basic standard that defines the rules of the internet and is a common protocol used to deliver data in digital network communications.

- The TCP/IP model consists of several types of protocols, including:
   - TCP and IP
   - Address Resolution Protocol (ARP)
   - Internet Control Message Protocol (ICMP)
   - Reverse Address Resolution Protocol (RARP)
   - User Datagram Protocol (UDP)

![tcpmod](https://gist.githubusercontent.com/Samsar4/62886aac358c3d484a0ec17e8eb11266/raw/bccff9a7c15aa11636c03686ef344ae2d433f699/tcpmodel.png)

<sub><sup>TCP/IP Model</sup></sub>

TCP is the most commonly used of these protocols and accounts for the most traffic used on a TCP/IP network. **UDP is an alternative to TCP that does not provide error correction, is less reliable, and has less overhead, which makes it ideal for streaming.**

## The User Datagram Protocol (UDP)
Is a lightweight data transport protocol that works on top of IP.
UDP provides a mechanism to detect corrupt data in packets, but it does not attempt to solve other problems that arise with packets, such as lost or out of order packets. That's why UDP is sometimes known as the Unreliable Data Protocol.
UDP is simple but fast, at least in comparison to other protocols that work over IP. It's often used for time-sensitive applications (such as real-time video streaming) where speed is more important than accuracy.

- On Linux and Unix systems you can issue the `lsof` command to see which processes is using UDP ports
![udp](https://cdn.kastatic.org/ka-perseus-images/edbdf593300fc4a51c60a97998c4d01a51ccd3b1.png)

## The TCP format
![tc](https://cdn.kastatic.org/ka-perseus-images/e5fdf560fdb40a1c0b3c3ce96f570e5f00fff161.svg)

## The UDP format
![udp](https://cdn.kastatic.org/ka-perseus-images/9d185d3d44c7ef1e2cd61655e47befb4d383e907.svg)

## TCP Handshake

TCP uses a three-way handshake to establish a reliable connection. The connection is full duplex, and both sides synchronize (SYN) and acknowledge (ACK) each other. The exchange of these four flags is performed in three steps:
1. SYN
2. SYN-ACK
3. ACK 

![3wayhandshake](https://gist.githubusercontent.com/Samsar4/62886aac358c3d484a0ec17e8eb11266/raw/bd38a6a2d83ea02a4715d6cb7fd8e0d74af3bd26/3wayhs.jpg)

The three message mechanism is designed so that two computers that want to pass information back and forth to each other can negotiate the parameters of the connection before transmitting data such as HTTP browser requests.

## More TCP Flags

| Flag | Name           | Function                                                     |
| ---- | -------------- | ------------------------------------------------------------ |
| SYN  | Synchronize    | Set during initial communication.  Negotiating of parameters and sequence numbers |
| ACK  | Acknowledgment | Set as an acknowledgement to the SYN flag.  Always set after initial SYN |
| RST  | Reset          | Forces the termination of a connection (in both directions)  |
| FIN  | Finish         | Ordered close to communications                              |
| PSH  | Push           | Forces the delivery of data without concern for buffering    |
| URG  | Urgent         | Data inside is being sent out of band.  Example is cancelling a message |

## Capturing 3 Way handshakes (Example)

- The figure below shows the 3-way-handshake packets captured by [Wireshark](https://www.wireshark.org/)

![wireshark](https://gist.githubusercontent.com/Samsar4/62886aac358c3d484a0ec17e8eb11266/raw/5213becc28e3f9f46c976d05cd090ffd070ff5d1/wireshark0.png)

# 5. Порты & Протоколы
## What is a Port?
In computer networking, a port is a communication endpoint. At the software level, within an operating system, a port is a logical construct that identifies a specific process or a type of network service.

## The most common ports
As a penetration tester or ethical hacker you should be familiar with the common ports and protocols used by popular services.

### <u>Port Numbers</u>

- **Internet Assigned Numbers Authority** (IANA) - maintains Service Name and Transport Protocol Port Number Registry which lists all port number reservations

- Ranges

  - **Well-known ports** - 0 - 1023

  - **Registered ports** - 1024 - 49,151

  - **Dynamic ports** - 49,152 - 65,535

    | Port Number | Protocol | Transport Protocol |
    | ----------- | -------- | ------------------ |
    | 20/21       | FTP      | TCP                |
    | 22          | SSH      | TCP                |
    | 23          | Telnet   | TCP                |
    | 25          | SMTP     | TCP                |
    | 53          | DNS      | TCP/UDP            |
    | 67          | DHCP     | UDP                |
    | 69          | TFTP     | UDP                |
    | 80          | HTTP     | TCP                |
    | 110         | POP3     | TCP                |
    | 135         | RPC      | TCP                |
    | 137-139     | NetBIOS  | TCP/UDP            |
    | 143         | IMAP     | TCP                |
    | 161/162     | SNMP     | UDP                |
    | 389         | LDAP     | TCP/UDP            |
    | 443         | HTTPS    | TCP                |
    | 445         | SMB      | TCP                |
    | 514         | SYSLOG   | UDP                |

  - A service is said to be **listening** for a port when it has that specific port open

  - Once a service has made a connection, the port is in an **established** state

  - **`netstat`** command:

    - Shows open ports on computer
    - **netstat -an** displays connections in numerical form
    - **netstat -b** displays executables tied to the open port (admin only)

# 6. Модель OSI
OSI Model is a hypothetical networking framework that uses specific protocols and mechanisms in every layer of it. This model is used to divide the network architecture into seven different layers conceptually. These layers are:

![osi-model](https://gist.githubusercontent.com/Samsar4/62886aac358c3d484a0ec17e8eb11266/raw/3e2dc59e7c341f4d79b2b93bac03fd8378c7ae3a/tcpmo.jpg)

There also involves some security postures and mechanisms that a security professional must know to detect and put the security method effectively in every layer.

## More about the Layers:

## Layer 7 - Application

![l7](https://www.cloudflare.com/img/learning/ddos/glossary/open-systems-interconnection-model-osi/7-application-layer.svg)

- This is the only layer that directly interacts with data from the user. Software applications like web browsers and email clients rely on the application layer to initiate communications. But it should be made clear that client software applications are not part of the application layer; rather the application layer is responsible for the protocols and data manipulation that the software relies on to present meaningful data to the user. Application layer protocols include HTTP as well as SMTP (Simple Mail Transfer Protocol is one of the protocols that enables email communications).

## Layer 6 - Presentation

![l6](https://www.cloudflare.com/img/learning/ddos/glossary/open-systems-interconnection-model-osi/6-presentation-layer.svg)

- This layer is primarily responsible for preparing data so that it can be used by the application layer; in other words, layer 6 makes the data presentable for applications to consume. The presentation layer is responsible for translation, encryption, and compression of data.

## Layer 5 - Session Layer

![l5](https://www.cloudflare.com/img/learning/ddos/glossary/open-systems-interconnection-model-osi/5-session-layer.svg)

- This is the layer responsible for opening and closing communication between the two devices. The time between when the communication is opened and closed is known as the session. The session layer ensures that the session stays open long enough to transfer all the data being exchanged, and then promptly closes the session in order to avoid wasting resources.

## Layer 4 - Transport Layer

![l4](https://www.cloudflare.com/img/learning/ddos/glossary/open-systems-interconnection-model-osi/4-transport-layer.svg)

- Layer 4 is responsible for end-to-end communication between the two devices. This includes taking data from the session layer and breaking it up into chunks called segments before sending it to layer 3. The transport layer on the receiving device is responsible for reassembling the segments into data the session layer can consume.

- The transport layer is also responsible for flow control and error control. Flow control determines an optimal speed of transmission to ensure that a sender with a fast connection doesn’t overwhelm a receiver with a slow connection. The transport layer performs error control on the receiving end by ensuring that the data received is complete, and requesting a retransmission if it isn’t.

## Layer 3 - Network Layer

![l3](https://www.cloudflare.com/img/learning/ddos/glossary/open-systems-interconnection-model-osi/3-network-layer.svg)

- The network layer is responsible for facilitating data transfer between two different networks. If the two devices communicating are on the same network, then the network layer is unnecessary. The network layer breaks up segments from the transport layer into smaller units, called packets, on the sender’s device, and reassembling these packets on the receiving device. The network layer also finds the best physical path for the data to reach its destination; this is known as routing.

## Layer 2 - Data Link Layer

![l2](https://www.cloudflare.com/img/learning/ddos/glossary/open-systems-interconnection-model-osi/2-data-link-layer.svg)

- The data link layer is very similar to the network layer, except the data link layer facilitates data transfer between two devices on the SAME network. The data link layer takes packets from the network layer and breaks them into smaller pieces called frames. Like the network layer, the data link layer is also responsible for flow control and error control in intra-network communication (The transport layer only does flow control and error control for inter-network communications).

## Layer 1 - Physical Layer

![l1](https://www.cloudflare.com/img/learning/ddos/glossary/open-systems-interconnection-model-osi/1-physical-layer.svg)

- This layer includes the physical equipment involved in the data transfer, such as the cables and switches. This is also the layer where the data gets converted into a bit stream, which is a string of 1s and 0s. The physical layer of both devices must also agree on a signal convention so that the 1s can be distinguished from the 0s on both devices.
