---
title: "Дампинг и установка DSiWare приложений"
permalink: /dumping-dsiware.html
author_profile: true
---

{% include toc title="Содержание" %}


Это руководство позволит снять дамп DSiWare приложений с 3ds для последующего использования на DSi.
Требуется наличие прошитой 3ds с установленными Luma3ds, GodMode и FBI. Следуйте [3ds.customfw.xyz](https://3ds.customfw.xyz){:target="_blank"} для взлома Вашей 3DS.
{: .notice--warning}


# Дампинг DSiWare приложений
Все шаги выплняются на 3ds
{: .notice--info}

## Нахождение TittleID DSiWare
1. Запустите `FBI` на Вашей 3DS
2. Выделите `Tittles` и нажмите ![]({{ "/images/buttons/A.png" | absolute_url }})
3. Нажмите ![]({{ "/images/buttons/SELECT.png" | absolute_url }}) и кнопкой ![]({{ "/images/buttons/A.png" | absolute_url }}) выделите пункты “Show game card” и “Show SD”
4. Нажмите ![]({{ "/images/buttons/B.png" | absolute_url }}) и дождитесь построения списка
5. Пролистайте список до нужного Вам DSiWare приложения
6. Запишите Title ID приложения с верхнего экрана консоли
7. Выключите 3ds

## Дампинг DSiWare
1. Включите 3DS с зажатой кнопкой ![]({{ "/images/buttons/START.png" | absolute_url }}) для запуска меню chainloader.
2. Выделите `GodMode9`  и нажмите ![]({{ "/images/buttons/A.png" | absolute_url }})
3. Перейдите в `[2:] SYSNAND TWLN/title/00030004`
4. Найдите нужное Вам приложение по последним 8 знакам Title ID и остановитесь на нём
5. Нажмите ![]({{ "/images/buttons/R.png" | absolute_url }}) + ![]({{ "/images/buttons/A.png" | absolute_url }})
6. Выберите “Copy to 0:/gm9/out”
7. Нажмите ![]({{ "/images/buttons/A.png" | absolute_url }}) по окончании копирования
8. Выключите консоль

Дамп Вашего приложения будет на SD-карте приставки в папке gm9/out. Скопируйте его на Ваш компьютер.

___

# Установка DSiWare приложений

У вас уже должны быть установлены [**Unlaunch**](get-started) и [**HiyaCFW**](installing-HiyaCFW)
{: .notice--warning}

Это руководство позволит установить снятые дампы DSiWare приложений в главное меню DSi.


## Что понадобится
- Свежая версия [maketmd](https://github.com/Tuxality/maketmd/releases){:target="_blank"}

## Инструкция
1. Скопируйте содержимое архива `maketmd.zip` в папку на Вашем компьютере
2. Откройте папку с дампом dsiware
3. Перейдите в папку `content`
4. Удалите папку `cmd` и файл `.tmd`
5. Удилите файлы `.ctx` если присутствуют
6. Перетащите файл `.app` на программу maketmd
- создастся новый файл - `title.tmd`
7. Скопируйте папку с дампом в папку `/title/00030004` SD-карты Вашей DSi
- Если системное меню было заменено на TWiLightMenu++, нужно будет перезапустить `launcharggen` и поместить новые файлы `launcharg` в `roms/dsiware` еще раз
8. Включите Вашу DSi и "распакуйте" новое приложение
- если консоль загрузится в экран “error has occured”, значит вы привысили лимит установленных dsiware приложений, TWiLightMenu++ может обойти этот лимит

При дампинге некоторых игр в папке `content` будут находиться два `.app` файла. Удалите тот, который весит несколько байт, а оставшемуся измените название на `00000000.app` и следуйте инструкции. 
{: .notice--info}

Через TWiLightMenu++ можно запускать любое DSiWare приложение, сконвертированное в формат `.nds`, просто закинув его в папку с ромами, как и любую ds игру.
{: .notice--success}

___

[**Полезные инструкции**](addons)
{: .notice--success}
