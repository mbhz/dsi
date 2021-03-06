---
title: "Установка Unlaunch"
permalink: /get-started.html
author_profile: true
---

{% include toc title="Содержание" %}

Прежде чем начать, рекомендуется проверить свою SD-карту на ошибки с помощью 
[H2testw (Windows)](https://3ds.customfw.xyz/h2testw-windows){:target="_blank"}, [F3 (Linux)](https://3ds.customfw.xyz/f3-linux){:target="_blank"}, или [F3X (Mac)](https://3ds.customfw.xyz/f3x-mac){:target="_blank"}<br>

Если вы пользователь **Windows**, то перед началом работ убедитесь, что в Вашей системе включено отображение расширений файлов. Если вы не знаете как это сделать, следуйте этой инструкции: [Расширения файлов (Windows)](https://3ds.customfw.xyz/file-extensions-windows){:target="_blank"}.

Если у Вас консоль **USA** региона, то убедитесь в том, что в настройках приставки выставлен английский язык.

Unlaunch - это эксплоит загрузочного кода DSi, позволяющий установить кастомную прошивку HiyaCFW на Вашу приставку.

## Что понадобится 
- [SD-card files](files/SD-card.zip)
- Memory Pit (pit.bin)
	- [Для версии системы 1.0 - 1.3 (USA, EUR, AUS, JPN)](files/memory_pit/10/pit.bin)
	- [Для версии системы 1.4 - 1.4.5 (USA, EUR, AUS, JPN)](files/memory_pit/14/pit.bin)
	- [Для версии системы 1.0 - 1.4.6 (KOR, CHN, iQue)](files/memory_pit/10/pit.bin)
	
## Подготовка SD карты
1. Запустите приложение **Камера** и выбирите SD-карту в правом верхнем углу, чтобы консоль создала нужные файлы
2. Выньте Вашу SD-карту из консоли и вставьте её в компьютер
3. Скопируйте содержимое архива `SD-card.zip` в корень Вашей SD-карты
4. Скопируйте файл `pit.bin` по пути `/private/ds/app/484E49##` (последние два знака зависят от региона консоли) с заменой, если спросит
5. Извлеките Вашу SD карту и вставьте её в DSi

## Создание бэкапа NAND 
1. Откройте приложение **Камера DSi**
- Выбирите SD-карту в правом верхнем углу
- Нажмине на кнопку с альбомом (правая)
		- Должно запуститься HBMenu
2. Выберите **fwtool.nds**
- Должен запуститься fwtool
3. Выберите **Backup DSi NAND**  
- процесс займет несколько минут
- Когда появится надпись `saved nand.bin.sha1.`, создание бекапа закончено.
4. Выберите **Exit** и выключите Вашу DSi.
5. Выньте SD-карту из консоли и вставьте ее в ПК.
	- **Сохраните созданный бекап на компьютере (папка /nds/FWхххххххххххх/), он будет необходим для дальнейшей установки HiyaCFW.**

## Установка
1. Извлеките SD-карту из компьютера и вставьте ее в консоль
2. Откройте приложение **Камера DSi**
- Выбирите SD-карту в правом верхнем углу
- Нажмине на кнопку с альбомом (правая)
		- Должно запуститься HBMenu
3. Выберите **unlaunch.nds**   
- Должен запуститься установщик Unlaunch
4. Выберите **INSTALL NOW**  
- Если Unlaunch завис с ошибкой **ERROR: MISMATCH IN FAT COPIES**, пожалуйста обратитесь к [FAQ](faq){:target="_blank"}
5. После завершения установки выберите **POWER DOWN**  
- Консоль выключится
6. Включите Вашу консоль для проверки работы Unlaunch
- Должен появиться экран меню Unlaunch
- Можно выключить консоль и извлеч SD-карту

___


Для восстановления функционала камеры, удалите скопированный вначале файл `pit.bin`.
{: .notice--info}

___

Далее, переходим к одному из пунктов установки, в зависимости от Ваших предпочтений: 


**TWiLightMenu ++** - приложение, заменяющее системное меню DSi. Позволяет запускать как ds/dsiware тайтлы, так и игры с консолей предыдущих поколений через встроенные эмуляторы. Имеет множество визуальных и технических настроек.

**hiyaCFW** - это кастомная прошивка, позволяющая запускать систему с SD-карты вместо внутренней памяти (аналог emunand/rednand на 3ds), что дает возможность устанавливать dsiware приложения непосредственно в родное меню dsi. Для запуска `.nds` тайтлов необходимо будет также использовать TWiLightMenu ++, которое буде установленно в процессе.


[**Установка TWiLightMenu ++**](twlmenu)
{: .notice--success}

[**Установка HiyaCFW**](installing-hiyaCFW)
{: .notice--success}