# Распознавание дорожных знаков
_Activate Sign Assist (Traffic Sing Recognition)_

**Блок 17** Комбинация приборов

*Длинное кодирование*

`Byte 05` `Bit 02` `Activate` -> (Sing Assist installed)

или

(что, то же самое для этого пункта):

**Блок 17** Комбинация приборов

*Адаптация*

`Распознавание дорожных знаков` Старое значение: `не акт.` Новое значение: `акт.`

**Блок A5** (front / advance camera)

Безопасный доступ, Логин: 20103

*Длинное кодирование*

`Byte 16` `Bit 04` `Activate` (Sing Assist aktive)

**Блок 5F** Information

*Адаптация*

`Car_Function_List_BAP_Gen2`

`traffic_sign_recognition_0x21` = `Activated`

`Car_Function_Adaptions_Gen2`

`menu_display_road_sign_identification` = `Activated`

`Car_Function_Adaptions_Gen2`
`menu_display_road_sign_identification_over_threshold_hidh` = `Activated`

В случае ошибки в [Блок 13 Адаптивный круиз-контроль (data bus)](../units/unit-13.md), необходима следующая кодировка:

**Блок 13** Адаптивный круиз-контроль

*Длинное кодирование*

`Byte 01` `Bit 00` -> `Activate`

_Примечание к комплексной кодировке_:

После данных активаций в ГУ в разделе **Автомобиль / Настройки** появятся пункты:
1. Ассистенты водителя:
   - Ассистент распознавания дорожных знаков
     * Отображать в комбинации приборов V
2. Комбинация приборов:
   - Ассистент распознавания дорожных знаков V
