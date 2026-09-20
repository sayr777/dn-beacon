# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Назначение репозитория

Портфолио лендингов для продажи коммерческих решений на базе промышленного образца BLE-метки [dynamic-iBeacon](https://github.com/sayr777/dynamic-iBeacon) (локально: `C:\T1_GIT\dynamic-ibeacon`).

## Структура проекта

```
dn-beacon/
├── index.html          # Главный каталог всех решений
├── dn-fleet/           # DN·Fleet — коммерческий транспорт и логистика
│   ├── index.html
│   └── README.md
├── dn-city/            # DN·City — общественный транспорт и умный город
│   ├── index.html
│   └── README.md
└── dn-road/            # DN·Road — дорожная отрасль и инфраструктура
    ├── index.html
    └── README.md
```

Смежный репозиторий: `C:\MY_GIT\ble-transit-payment` (DN·Pay — оплата проезда).  
Все `index.html` — самодостаточные одностраничники без зависимостей, готовые к публикации на GitHub Pages или любом статическом хостинге.

## Аппаратная платформа (справка)

| Параметр | Значение |
|---|---|
| Чипсет | Nordic nRF52832 (модуль YJ-16013) |
| Батарея | ER14505H-LD, Li-SOCl₂, 2700 мАч |
| Срок жизни батареи | 15–20 лет (~5.2 µА день, ~1.1 µА ночь) |
| Корпус | AK-W-70-4, IP67, 70×40×20 мм, −40…+85°C |
| Безопасность | AES-128 ECB, Major/Minor/MAC меняются каждые 5 мин |
| Дальность | до 70 м (регулируется TX power) |
| Протокол | стандартный iBeacon (BLE 4.0+) |

## Публикация

Для GitHub Pages достаточно включить Pages на ветке `master`/`main` с корневой папкой `/`.  
Каждая подпапка (`dn-fleet/`, `dn-city/`, `dn-road/`) публикуется по соответствующему пути.
