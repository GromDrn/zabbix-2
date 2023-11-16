# Домашнее задание к занятию "`Система мониторига Zabbix 2`" - `Громов Андрей`

---

### Задание 1

Template:
![Скриншот-1](https://github.com/GromDrn/zabbix-2/blob/main/Screenshots/1-Template.jpg)

---

### Задание 2 - 3


Template:
![Скриншот-1](https://github.com/GromDrn/zabbix-2/blob/main/Screenshots/2-3_Templ%20_my.png)

---
Status OK:
![Скриншот-2](https://github.com/GromDrn/zabbix-2/blob/main/Screenshots/2-3_Status_OK.jpg)

---
CPU & RAM:
![Скриншот-3](https://github.com/GromDrn/zabbix-2/blob/main/Screenshots/2-3_CPU%26RAM_value.png)

---

### Задание 4


Dashboard:
![Скриншот-1](https://github.com/GromDrn/zabbix-2/blob/main/Screenshots/4-Dash.png)


### Задание 5

MAP:
![Скриншот-1](https://github.com/GromDrn/zabbix-2/blob/main/Screenshots/5-MAP.jpg)


### Задание 6

```bash
!/bin/bash
if [ "$1" = "1" ]; then
    echo "Gromov AA"
  elif [ "$1" = "2" ]; then
    echo "$(date)"
  else
    echo "Unknown argument"
fi
``` 

Latest Data:
![Скриншот-1](https://github.com/GromDrn/zabbix-2/blob/main/Screenshots/6-Latest_data.png)


### Задание 7

```python

import sys
import os
import re
import datetime

if (sys.argv[1] == '-ping'):
        result=os.popen("ping -c 1 " + sys.argv[2]).read()
        result=re.findall(r"time=(.*) ms", result)
        print(result[0])
elif (sys.argv[1] == '-simple_print'):
    if sys.argv[2] == "1":
         print("Gromov AA")
    elif sys.argv[2] == "2":
         print(datetime.datetime.now())
    else:
         print(sys.argv[2])     
else: 
    print(f"unknown input: {sys.argv[1]}")
``` 

Items setup:
![Скриншот-1](https://github.com/GromDrn/zabbix-2/blob/main/Screenshots/7-Items_setup.png)

---

Latest Data:
![Скриншот-2](https://github.com/GromDrn/zabbix-2/blob/main/Screenshots/7-Latest_Data.jpg)



### Задание 8


Rules:
![Скриншот-1](https://github.com/GromDrn/zabbix-2/blob/main/Screenshots/8%20rules.png)

Discovery:
![Скриншот-2](https://github.com/GromDrn/zabbix-2/blob/main/Screenshots/8%20diskovery.png)


