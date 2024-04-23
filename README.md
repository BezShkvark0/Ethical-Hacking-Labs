# <p align="center">Этичный Хакинг
</p>

![h](https://gist.githubusercontent.com/Samsar4/62886aac358c3d484a0ec17e8eb11266/raw/89f706846f97cd3e59880dbc03e4f1d5f8023783/header-ehl.jpg)

* * *

> **⚠️ ДИСКЛЕЙМЕР**:
*Данный репозиторий является ни чем инным как "фанатской" адоптацией(локализцией) [оригинального репозитория](https://github.com/Samsar4/Ethical-Hacking-Labs) на русский язык.*

* * * 

Данная подборка туториалов и лаб сделана сугубо для людей изучающих этичный хакинг, кибербезопасность, сеть и системное администрирование. Эти туториалы приводят информацию содержащуюся на [CEH](https://www.eccouncil.org/train-certify/certified-ethical-hacker-ceh-v12/) и прочих источников из интернета.

⌨️ Данные туториалы ориентированы на практическую составляющую. Не волнуйтесь, если вы полный нуб, вам не нужно быть техножрецом 80+ лвл, чтобы начать изучение этичного хакинга. **Помните, Гугл - ваш лучши друг.** Этот репозиторий проведёт вас по пути от самых основ до более продвинутых приёмов.

**✅ Системные требования**:
* Любой компьютер с как минимум 8ГБ RAM (рекомендуется 16ГБ)
* Хотя бы 80ГБ свободного места на вашем жёстком диске
* Аппаратная поддержка виртуализации

* * *

> **⚠️ Дисклеймер**:
*Данный материал предоставлен сугубо в академических целях. НЕ используйте следующие техники в любых публичных сетях. Потому как, если вас признают виновным в причинении какого-либо вреда какому-либо лицу, правительству, корпоративному органу, некоммерческой организации и т. д., вам будет предъявлен иск по обвинению в киберпреступлении/ях. Я рекомендую вам попрактиковаться в уроках этого курса на вашей собственной системе и ваших собственных данных в частной или локальной сети.*

* * * 

## ⚙️ Базовые знания
Итак, для начала вам нужно разобраться как всё работает, прежде чем приступать к разборке и поиску уязвимостей. Чем больше вы поймёте, тем более хорошим хацкером вы станете. "Базовые знания" (модуль 0) представляет собой быстрый ввод в курс дела.

**Базовые знания содержат введение по работе с сетями, системами Linux, виртуализацией, созданием лабораторий, написанием скриптов, а также темами информационной безопасности. Если вы знакомы с этими темами, вы можете сразу перейти к модулю Этического взлома.**

* [Сеть 101](/0-Core-Knowledge/0-Networking-101.md)
* [Создание Лаборатории / Виртуализация](/0-Core-Knowledge/1-Lab-Building.md)
* [Введение в Linux](/0-Core-Knowledge/2-Intro-to-Linux.md)
* [Скриптование]()
* [Информационная Безопасность 101](/0-Core-Knowledge/4-Infosec-101.md)

## ⚔️ Этичный Хакинг
1. **Футпринтинг и Разведка**
    * [Введение](/1-Footprinting-and-Reconnaissance/0-What-is-Footprinting.md)
    * [Командная строка Windows](/1-Footprinting-and-Reconnaissance/1-Windows-CommandLine.md)
    * [Основы Maltego](/1-Footprinting-and-Reconnaissance/2-Maltego-Basics.md)
    * [Recon-ng](/1-Footprinting-and-Reconnaissance/3-Recon-ng.md)
    * [OSRFramework](/1-Footprinting-and-Reconnaissance/4-OSRFramework.md)
    * [Metasploit](/1-Footprinting-and-Reconnaissance/5-Metasploit-Basics.md)
    * [theHarvester](/1-Footprinting-and-Reconnaissance/6-theHarvester.md)
    * [Прочие инструменты для Разведки](/1-Footprinting-and-Reconnaissance/7-Other-Tools.md)
2. **Сканирование Сетей**
    * [Введение](/2-Scanning-Networks/0-Scanning-a-Target-Network.md)
    * [hping3](/2-Scanning-Networks/1-hping3.md)
    * [Определение ОС по TTL при помощи Wireshark](/2-Scanning-Networks/2-TTL.md)
    * [Mega Ping](/2-Scanning-Networks/3-MegaPing.md)
    * [Основы Nmap](/2-Scanning-Networks/4-Nmap.md)
    * [Избегаем обнаружения при помощи Nmap](/2-Scanning-Networks/5-NmapDecoyIP.md)
    * [Дополнительный графический инстурментарий Windows](/2-Scanning-Networks/6-WindowsTools.md)
3. **Перечисление**
    * [Введение](/3-Enumeration/0-Introduction.md)
    * [Перечисление при помощи Nmap](/3-Enumeration/1-Enumerating-with-Nmap.md)
    * [Перечисление SNMP](/3-Enumeration/2-SNMP-Enumeration.md)
    * [Enum4Linux](/3-Enumeration/3-Enum4linux-Win-and-Samba-Enumeration.md)
    * [Дополнительный графический инстурментарий Windows](/3-Enumeration/4-Windows-EnumerationTools.md)
4. **Анализ Уязвимостей**
    * [Обзор и Инструментарий](/4-Vulnerability-Analysis/Overview-and-Tools.md) 
5. **Взлом Систем**
    * [Введение](/5-System-Hacking/0-Introduction.md)
    * [Подмена LLMNR / NBT-NS](/5-System-Hacking/1-LLMNR-NBT-NS.md)
    * [Создание дампа and взлом SAM хэша](/5-System-Hacking/2-SAM-Hashes.md)
    * [Вскрываем пароли с RainbowCrack](/5-System-Hacking/3-Rainbow-tables.md)
    * [Создание сессии VNC](/5-System-Hacking/4-VNC-Session.md)
    * [Повышаем уровень доступа](/5-System-Hacking/5-Escalating-Privileges.md)
    * [Взлом Windows через файл MS Word](/5-System-Hacking/6-Hacking-Windows-with-Doc-file.md)
    * [Взлом Windows с Msf/Meterpreter - Постэксплойт](/5-System-Hacking/7-Hacking-Windows-with-Metasploit-PostExploitation.md)
    * [Прячем файлы - NTFS потоки](/5-System-Hacking/8-NTFS-Streams.md)
    * [Прячем файлы - Стеганография](/5-System-Hacking/9-Steganography.md)
    * [Использование Covert_TCP](/5-System-Hacking/10-Covert_TCP.md)
    * [Основы Auditpol](/5-System-Hacking/11-Auditpol.md)
    * [Дополнительный графический инстурментарий Windows](/5-System-Hacking/12-WindowsTools.md)
6. **Вирусня** 
    * [Введение](/6-Malware/0-Introduction.md)
    * [njRAT](/6-Malware/1-Using-njRAT.md)
    * [HTTP RAT Троян](/6-Malware/2-HTTP-Trojan.md)
    * [Скрываем Троян с помощью SwayzCryptor](/6-Malware/3-Obfuscating-Trojan-SwayzCryptor.md)
    * [Лаба для анализа вирусни](/6-Malware/4-Malware-Analysis-Lab.md)
    * [Инструментарий для Windows](/6-Malware/5-Windows-Tools.md)
7. **Сниффинг**
    * [Введение](/7-Sniffing/0-Introduction.md)
    * [MITM атака с помощью BetterCAP](/7-Sniffing/1-MITM-with-Bettercap.md)
    * [MAC адресс Спуфинг](/7-Sniffing/2-Spoofing-MAC-address.md)
    * [Инструментарий для Windows](/7-Sniffing/x-Windows-Tools.md)
8. **Социальныя инженерия**
    * [Введение](/8-Social-Engineering/0-Introduction.md)
    * [Использования SET](/8-Social-Engineering/1-Using-SET.md)
    * [Инструментарий](/8-Social-Engineering/X-Tools.md)
9. **DoS атака**
    * [Введение](/9-Denial-of-Service/0-Introduction.md)
    * [SYN Флудинг](/9-Denial-of-Service/1-SYN-Flooding.md)
    * [DDoS с помощью HOIC](/9-Denial-of-Service/2-DDoS-using-HOIC.md)
    * [Обнаружение трафика атаки DoS](/9-Denial-of-Service/3-Detecting-DoS-Traffic.md)
10. **Сессионное перехватывание**
    * [Введение](/10-Session-Hijacking/0-Introduction.md)
    * [Использование ZAP - Zed Attack Proxy](/10-Session-Hijacking/1-Using-ZAP.md)
    * [Перехват HTTP трафика](/10-Session-Hijacking/2-Intercepting-HTTP-Traffic.md)
11. **Бонус - 🔬 Метод суд-мед эксперта**
    * [TCPDump](/11-Bonus/TCPDump-Tutorial.md)
    * [Анализ Пакетов](/11-Bonus/Dissecting-packets.md)
    * [ExifTool](/11-Bonus/ExifTool-Tutorial.md)
    * [hdparm & dd команды](/11-Bonus/Using-hdparm-and-dd-command.md)
    * [Восстановление удалённого раздела](/11-Bonus/Recovering-Deleted-Partition.md)
    * [Восстановление удалённых файлов](/11-Bonus/Recovering-Deleted-Files.md)

* * * 

**💭 To Do**:
- ![](https://img.shields.io/badge/status-in%20progress-orange)
- Add Foundational level modules (~~networking~~, ~~virtualization~~, crypto, linux kernel and scripting).
- Bonus modules to add:
    - ~~Introduction to Infosec terms and methodologies (from [CEH Study Guide](https://github.com/Samsar4/CEH-v10-Study-Guide))~~
    - More Reconnaissance techniques.
    - Active Directory: Lab build and attack vectors.
    - Web application: Enumeration and exploitation using some OWASP Top 10 vulnerabilities and Bug Bounty techniques.
    - Wireless hacking (WPA)
