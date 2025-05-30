---
title: OnVehicleSpawn
sidebar_label: OnVehicleSpawn
description: Ова повратна функција се позива када се возило респаунује.
tags: ["vehicle"]
---

:::warning

Ова повратна функција се позива **само** када се возило **респаунује**! `CreateVehicle` и `AddStaticVehicle(Ex)` **неће** активирати ову повратну функцију.

:::

## Опис

Ова повратна функција се позива када се возило респаунује.

| Име       | Опис                                |
| --------- | ----------------------------------- |
| vehicleid | ID возила које је респаунујемо.     |

## Враћа

**0** - Спречиће друге филтер скрипте да приме ову повратну функцију.

**1** - Индикатор да ће ова повратна функција бити прослеђена другим филтер скриптама.

Увек се позива први у филтер скриптама.

## Приемри

```c
public OnVehicleSpawn(vehicleid)
{
    printf("Vehicle %i spawned!",vehicleid);
    return 1;
}
```

## Повезане повратне функције

Следеће повратне функције могу бити корисне, јер су на неки начин повезане са овом повратном функцијом.


- [OnVehicleDeath](OnVehicleDeath): Ова повратна функција се позива када се возило уништи.
- [OnPlayerSpawn](OnPlayerSpawn): Ова повратна функција се позива када се играч спаун-ује.

## Повезане функције

Следеће функције могу бити корисне, јер су на неки начин повезане са овом повратном функцијом.

- [SetVehicleToRespawn](../functions/SetVehicleToRespawn): Респавнује возило.
- [CreateVehicle](../functions/CreateVehicle): Креира возило.
