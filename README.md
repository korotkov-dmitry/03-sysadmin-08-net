# Домашнее задание к занятию "3.8. Компьютерные сети, лекция 3"

## 1. Подключитесь к публичному маршрутизатору в интернет. Найдите маршрут к вашему публичному IP
```
telnet route-views.routeviews.org
Username: rviews
show ip route x.x.x.x/32
show bgp x.x.x.x/32
```

Результат:

`route-views>show ip route 176.50.168.66
Routing entry for 176.50.0.0/16
  Known via "bgp 6447", distance 20, metric 0
  Tag 6939, type external
  Last update from 64.71.137.241 1w1d ago
  Routing Descriptor Blocks:
  * 64.71.137.241, from 64.71.137.241, 1w1d ago
      Route metric is 0, traffic share count is 1
      AS Hops 2
      Route tag 6939
      MPLS label: none`
## 2. Создайте dummy0 интерфейс в Ubuntu. Добавьте несколько статических маршрутов. Проверьте таблицу маршрутизации.

## 3. Проверьте открытые TCP порты в Ubuntu, какие протоколы и приложения используют эти порты? Приведите несколько примеров.

## 4. Проверьте используемые UDP сокеты в Ubuntu, какие протоколы и приложения используют эти порты?

## 5. Используя diagrams.net, создайте L3 диаграмму вашей домашней сети или любой другой сети, с которой вы работали. 
