---
date: 2019-03-14 10:00:00 -0300
title: Отладка Push Notification в Android
categories:
  - chudnyi
description: Отладка Push Notification в Android
type: Document
author: chudnyi
---

- Отправить тестовый пуш можно из [Postman \| Download Postman App](https://go.dmit.ch/2O3homd)
- Описание способа: [Test FCM Notification with POSTMAN\! – Android School – Medium](https://go.dmit.ch/2O4QPNt)
- Документация: [Firebase Cloud Messaging HTTP protocol  \|  Firebase](https://go.dmit.ch/2O11TLm)

Необходимо получить два параметра: 
- ключ сервера приложения firebase
![firebase server token](http://cdn.chudnyi.com/assets/2019-03-14-mnsp-e81vp.png)

- токен устройства, уникальный ID устройства, отправляется устроству в рантайме при регистрации устройства в сервисе пушей
![push device token](http://cdn.chudnyi.com/assets/2019-03-14-mnsp-pm3ew.png)

#### Отправка сообщения

![headers](http://cdn.chudnyi.com/assets/2019-03-14-mnsp-1kiz3.png)
![body](http://cdn.chudnyi.com/assets/2019-03-14-mnsp-7j6xt.png)

больше параметров сообщения см. в документации
