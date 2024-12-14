---
authors:
  - FlashYan123
---

# Geyser: Bukkit

## Что это такое? {#what}

Geyser — это мост между Java и Bedrock версиями майнкрафта. Он позволяет игрокам с Bedrock подключаться на Java. Есть несколько версий Geyser, но в этой статье будет затронута только его Bukkit версия.

## Установка и настройка плагина Geyser {#install-and-setup}

:::info Заметка
Плагин требует дополнительный порт!
:::

### Шаг 1: Установка на сервер

1. Скачайте [плагин](https://geysermc.org/download);
2. [Дальше выполняем действия из данной статьи](/minecraft/installplugins).

### Шаг 2: Настройка плагина Geyser

После установки плагина, вам необходимо настроить его под свои нужды. В папке `~/plugins/Geyser-Spigot` найдите файл `config.yml` и откройте его в любом текстовом редакторе.

Пример конфигурации:

```yaml
bedrock:
  address: 0.0.0.0
  port: 19132 (вписывайте сюда свой порт)
remote:
  address: 127.0.0.1
  port: 25565 (вписывайте сюда свой порт)
  auth-type: online
```

[Для более расширенной настройки, обратитесь к вики Geyser](https://wiki.geysermc.org/geyser/understanding-the-config/)

## Использование Geyser с Floodgate {#floodgate}

Floodgate — это дополнение к Geyser, которое позволяет игрокам Bedrock Edition подключаться к серверам Java Edition с Geyser, не имея аккаунта Xbox. Это особенно полезно, если на сервере используется оффлайн-режим.

### Установка Floodgate

Установка идентична установке Geyser, [скачать его можно тут](https://geysermc.org/download#floodgate).

### Настройка Geyser и Floodgate

После установки Floodgate, необходимо настроить Geyser для работы с ним. Найдите параметр `authtype` и измените его значение на `floodgate`.

Пример конфигурации:

```yaml
bedrock:
  address: 0.0.0.0
  port: 19132 (вписывайте сюда свой порт)
remote:
  address: 127.0.0.1
  port: 25565 (вписывайте сюда свой порт)
  auth-type: floodgate
```
