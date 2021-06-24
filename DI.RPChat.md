# RPChat

* Commands
  * __*Тип данных:*__ ```List<Command>```
  * __*Описание:*__ <br> Список возможных "команд".<br>
  __Help__ - описание "команды", которое указывается, когда игрок пишет: __*!rp chat help*__ (```string```)<br>
  __StartSymbols__ - если игрок начнёт сообщение с этих символов, то выполнится блок данной "команды". (```string```)<br>
  __Distance__ - радиус круга с центром в позиции игрока, внутри которого сообщение будет видно другим игрокам. (```float```)<br>
  __StandardFormat__ - формат "команды", который появляется по умолчанию. (```string/null```)<br>
  __HasChanceToFail__ - имеет ли "команда" возможность написать иной формат собщения. Шанс - 50/50. (```true/false```)<br>
  __FailureFormat__ - формат, который показывается при неудаче. Изначально сделан для подобия /try (```string/null```)<br>
  * __*Значение по умолчанию:*__ 
```
"Commands": [
    {
      "Help": "Обычный /me",
      "StartSymbols": "*",
      "Distance": 50.0,
      "StandardFormat": "{0}: <color=yellow>*{1}*</color>",
      "HasChanceToFail": false,
      "FailureFormat": null
    },
    {
      "Help": "Обычный /try",
      "StartSymbols": "**",
      "Distance": 50.0,
      "StandardFormat": "{0}: <color=yellow>*{1}*</color> <color=green>(Удачно)</color>",
      "HasChanceToFail": true,
      "FailureFormat": "{0}: <color=yellow>*{1}*</color> <color=red>(Неудачно)</color>"
    },
    {
      "Help": "Обычный /do",
      "StartSymbols": "***",
      "Distance": 55.0,
      "StandardFormat": "{0}: <color=yellow>*{1}*</color>",
      "HasChanceToFail": false,
      "FailureFormat": null
    },
    {
      "Help": "Обычный /whisper",
      "StartSymbols": ".",
      "Distance": 3.5,
      "StandardFormat": "{0}: <color=grey>*шепчет* {1}...</color>",
      "HasChanceToFail": false,
      "FailureFormat": null
    }
  ]
```

# Полезная информация
* Ссылка на видео-демонстрацию: [Видео]
