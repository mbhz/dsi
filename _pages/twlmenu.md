---
title: "Установка TWiLightMenu ++"
permalink: /twlmenu.html
author_profile: true
---

{% include toc title="Содержание" %}


У вас уже должен быть установлен [**Unlaunch**](get-started), перед продолжением
{: .notice--warning}


## Что понадобится
- Свежая версия [TWiLightMenu ++](https://github.com/DS-Homebrew/TWiLightMenu/releases/){:target="_blank"} 

	
## Инструкция
1. Распакуйте **TWiLightMenu.7z** в удобное вам место.
2. Скопируйте файл `boot.nds` и папку `_nds`  из `DSi&3DS - SD card users` в корень Вашей SD-карты
	- согласитесь на замену файла `boot.nds`
3. Скопируйте папку `_nds` в корень Вашей SD-карты, соглашаясь на объединение
	- пользователям macOS выбрать "слияние"
4. Скопируйте папку `roms` в корень Вашей SD-карты	
5. Извлеките Вашу SD-карту и вставьте ее в DSi
6. Включите консоль, зажав кнопки ![]({{ "/images/buttons/A.png" | absolute_url }}) и ![]({{ "/images/buttons/B.png" | absolute_url }})
- появится экран меню Unlaunch
7. Выберите **OPTIONS**
8. Выберите **NO BUTTON**
9. Из списка выберите **TWiLightMenu++**
- на нижнем экране в строке пути до файла отобразится sdmc:/BOOT.NDS 
10. Выберите **SAVE & EXIT**
11. Выключите консоль и включите снова
- должно запуститься **TWiLightMenu ++**

## Использование
1. Скопируйте ромы в соответствующие им папки на SD-карте консоли:
	- Game Boy и Game Boy Color ромы в папку `/roms/gb`, GBA ромы в папку `/roms/gba`, DS ромы в папку `/roms/nds` и т.д. 
	- Для запуска GBA ромов нужен биос от GBA, помещенный в корень SD-карты / папку `gba` / `_gba` под именем `"bios.bin"`
		- Существует 3 способа сдампить BIOS: с помощью [модифицированного GameCube/Wii](https://github.com/FIX94/gba-link-cable-dumper){:target="_blank"}, [GBA/DS Phat/DS Lite и GBA флешкартриджа](https://glazedbelmont.github.io/gbabiosdump/#gameboy-advance-sp-micro-ds-ds-lite){:target="_blank"}, [модифицированной 3DS с установленной NES/SNES virtual console игрой](https://glazedbelmont.github.io/gbabiosdump/#virtual-console-title-from-a-3ds){:target="_blank"}	


		
____

[**Полезные инструкции**](addons)
{: .notice--success}
		
