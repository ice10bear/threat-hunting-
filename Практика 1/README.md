------------------------------------------------------------------------

title: “Lab_1”

format:

md:

    output-file: readme.md

editor_options:

chunk_output_type: inline

------------------------------------------------------------------------

# Системы аутентификации и защиты от несанкционированного доступа

Лабораторная работа №1

## Цель

Вывести информацию о системе

## Исходные данные

1.  ОС Windows 10
2.  RStudio Desktop
3.  WSL2
4.  Интерпретатор языка R 4.2.2

## План

1.  Выполнить команду uname -r
2.  Выполнить команду cat /proc/cpuinfo | grep “model name”
3.  Выполнить команду journalctl -q -b | tail -n 30

## Шаги

1.  Сначала выполним команду uname -r для вывода информации о системе

``` bash
uname -r
```

    3.3.6-341.x86_64

2\. Далее команда cat /proc/cpuinfo | grep “model name” для вывода
информации о процессоре, строки которой содержат “model name”

``` bash
cat /proc/cpuinfo | grep "model name"
```

    model name  : 11th Gen Intel(R) Core(TM) i3-1115G4 @ 3.00GHz
    model name  : 11th Gen Intel(R) Core(TM) i3-1115G4 @ 3.00GHz
    model name  : 11th Gen Intel(R) Core(TM) i3-1115G4 @ 3.00GHz
    model name  : 11th Gen Intel(R) Core(TM) i3-1115G4 @ 3.00GHz

3\. Также выполним команду systeminfo для вывода основных сведений о
системе

``` bash
systeminfo
```


    Host Name:                 DESKTOP-1G5EMRG
    OS Name:                   Microsoft Windows 10 Home
    OS Version:                10.0.19045 N/A Build 19045
    OS Manufacturer:           Microsoft Corporation
    OS Configuration:          Standalone Workstation
    OS Build Type:             Multiprocessor Free
    Registered Owner:          Maxa
    Registered Organization:   
    Product ID:                00326-30000-00001-AA702
    Original Install Date:     05.09.2021, 20:09:27
    System Boot Time:          21.02.2023, 5:18:02
    System Manufacturer:       ASUSTeK COMPUTER INC.
    System Model:              VivoBook_ASUSLaptop X513EA_F513EA
    System Type:               x64-based PC
    Processor(s):              1 Processor(s) Installed.
                               [01]: Intel64 Family 6 Model 140 Stepping 1 GenuineIntel ~2995 Mhz
    BIOS Version:              American Megatrends International, LLC. X513EA.308, 27.07.2021
    Windows Directory:         C:\Windows
    System Directory:          C:\Windows\system32
    Boot Device:               \Device\HarddiskVolume1
    System Locale:             ru;Russian
    Input Locale:              ru;Russian
    Time Zone:                 (UTC+03:00) Moscow, St. Petersburg
    Total Physical Memory:     7 874 MB
    Available Physical Memory: 1 198 MB
    Virtual Memory: Max Size:  29 001 MB
    Virtual Memory: Available: 17 534 MB
    Virtual Memory: In Use:    11 467 MB
    Page File Location(s):     C:\pagefile.sys
    Domain:                    WORKGROUP
    Logon Server:              \\DESKTOP-1G5EMRG
    Hotfix(s):                 18 Hotfix(s) Installed.
                               [01]: KB5022502
                               [02]: KB5000736
                               [03]: KB5012170
                               [04]: KB5015684
                               [05]: KB5023696
                               [06]: KB5006753
                               [07]: KB5007273
                               [08]: KB5011352
                               [09]: KB5011651
                               [10]: KB5014032
                               [11]: KB5014035
                               [12]: KB5014671
                               [13]: KB5015895
                               [14]: KB5016705
                               [15]: KB5018506
                               [16]: KB5020372
                               [17]: KB5022924
                               [18]: KB5005699
    Network Card(s):           5 NIC(s) Installed.
                               [01]: Intel(R) Wireless-AC 9462
                                     Connection Name: Беспроводная сеть
                                     DHCP Enabled:    Yes
                                     DHCP Server:     192.168.88.1
                                     IP address(es)
                                     [01]: 192.168.88.208
                                     [02]: fe80::222c:b53:c43e:d9cc
                               [02]: Bluetooth Device (Personal Area Network)
                                     Connection Name: Сетевое подключение Bluetooth
                                     Status:          Media disconnected
                               [03]: TAP-Windows Adapter V9
                                     Connection Name: Ethernet 3
                                     Status:          Media disconnected
                               [04]: TAP-Windows Adapter V9
                                     Connection Name: Ethernet 2
                                     Status:          Media disconnected
                               [05]: VirtualBox Host-Only Ethernet Adapter
                                     Connection Name: Ethernet 4
                                     DHCP Enabled:    No
                                     IP address(es)
                                     [01]: 192.168.56.1
                                     [02]: fe80::faba:f082:8189:8e3a
    Hyper-V Requirements:      VM Monitor Mode Extensions: Yes
                               Virtualization Enabled In Firmware: Yes
                               Second Level Address Translation: Yes
                               Data Execution Prevention Available: Yes

## Оценка результата

В результате лабораторной работы мы получили основную информацию об ОС,
процессоре.

## Вывод

Таким образом, мы научились работать с базовыми командами Linux и
Windows и получать информацию об операционной системе.
