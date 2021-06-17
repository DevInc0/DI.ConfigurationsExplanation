# RPChat

* Commands
  * __*Тип данных:*__ ```List<Command>```
  * __*Описание:*__ <br> Список возможных "команд".<br>
  Help - Описание "команды", которое указывается, когда игрок пишет: __*!rp chat help*__ (```string/null```)<br>
  StartSymbols - начальные символы "команды", если игрок начнёт сообщение с этих символов, то выполнится блок данной "команды". (```string/null```)<br>
  VisibleRadius - радиус круга с центром в позиции игрока, внутри которого будет отправляться сообщение другим игрокам. (```float```)<br>
  StandardFormat - формат "команды", который появляется по умолчанию. (```string/null```)<br>
  HasChanceToFail - имеет ли "команда" возможность написать иной формат собщения. Шанс - 50/50. (```true/false```)<br>
  FailureFormat - второй формат, который показывается при неудаче. Изначально сделан для подобия /try (```string/null```)<br>
  * __*Значение по умолчанию:*__ 
```
"Commands": [
    {
      "Help": "Обычный /me",
      "StartSymbols": "*",
      "VisibleRadius": 50.0,
      "StandardFormat": "{0}: <color=yellow>*{1}*</color>",
      "HasChanceToFail": false,
      "FailureFormat": null
    },
    {
      "Help": "Обычный /try",
      "StartSymbols": "**",
      "VisibleRadius": 50.0,
      "StandardFormat": "{0}: <color=yellow>*{1}*</color> <color=green>(Удачно)</color>",
      "HasChanceToFail": true,
      "FailureFormat": "{0}: <color=yellow>*{1}*</color> <color=red>(Неудачно)</color>"
    },
    {
      "Help": "Обычный /do",
      "StartSymbols": "***",
      "VisibleRadius": 55.0,
      "StandardFormat": "{0}: <color=yellow>*{1}*</color>",
      "HasChanceToFail": false,
      "FailureFormat": null
    },
    {
      "Help": "Обычный /whisper",
      "StartSymbols": ".",
      "VisibleRadius": 3.5,
      "StandardFormat": "{0}: <color=grey>*шепчет* {1}...</color>",
      "HasChanceToFail": false,
      "FailureFormat": null
    }
  ]
```

