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

    `route-views>show bgp 176.50.168.66
    BGP routing table entry for 176.50.0.0/16, version 1388607817
    Paths: (24 available, best #23, table default)
      Not advertised to any peer
      Refresh Epoch 1
      4901 6079 3356 12389
        162.250.137.254 from 162.250.137.254 (162.250.137.254)
          Origin IGP, localpref 100, valid, external
          Community: 65000:10100 65000:10300 65000:10400
          path 7FE0E255C020 RPKI State valid
          rx pathid: 0, tx pathid: 0
      Refresh Epoch 3
      3303 12389
        217.192.89.50 from 217.192.89.50 (138.187.128.158)
          Origin IGP, localpref 100, valid, external
          Community: 3303:1004 3303:1006 3303:1030 3303:3056
          path 7FE14990EA18 RPKI State valid
          rx pathid: 0, tx pathid: 0
      Refresh Epoch 1
      7660 2516 12389
        203.181.248.168 from 203.181.248.168 (203.181.248.168)
          Origin IGP, localpref 100, valid, external
          Community: 2516:1050 7660:9001
          path 7FE0295D4370 RPKI State valid
          rx pathid: 0, tx pathid: 0
      Refresh Epoch 1
      3267 1299 12389
        194.85.40.15 from 194.85.40.15 (185.141.126.1)
          Origin IGP, metric 0, localpref 100, valid, external
          path 7FE0A9BCBFD8 RPKI State valid
          rx pathid: 0, tx pathid: 0
      Refresh Epoch 1
      57866 3356 12389
        37.139.139.17 from 37.139.139.17 (37.139.139.17)
          Origin IGP, metric 0, localpref 100, valid, external
          Community: 3356:2 3356:22 3356:100 3356:123 3356:501 3356:901 3356:2065
          path 7FE0A9981800 RPKI State valid
          rx pathid: 0, tx pathid: 0
      Refresh Epoch 1`
## 2. Создайте dummy0 интерфейс в Ubuntu. Добавьте несколько статических маршрутов. Проверьте таблицу маршрутизации.

## 3. Проверьте открытые TCP порты в Ubuntu, какие протоколы и приложения используют эти порты? Приведите несколько примеров.

## 4. Проверьте используемые UDP сокеты в Ubuntu, какие протоколы и приложения используют эти порты?

## 5. Используя diagrams.net, создайте L3 диаграмму вашей домашней сети или любой другой сети, с которой вы работали. 
