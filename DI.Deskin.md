# Deskin

* AdminByPass
  * __*Тип данных:*__ ```bool```
  * __*Значение по умолчанию:*__ ```false```
  * __*Описание:*__ Пропускать ли "синих" админов.
  
* BlockedSkins
  * __*Тип данных:*__ ```Dictionary<string, bool>```  
  * __*Описание:*__ Список скинов, которые нужно заблокировать (```true``` - заблокировать; ```false``` - не блокировать) <br>
  **Items** - скины оружия, предметов. <br>
  **Hat** - скин головного убора. <br>
  **Mask** - скин маски. <br>
  **Glasses** - скин очков. <br>
  **Shirt** - скин куртки. <br>
  **Vest** - скин жилета. <br>
  **Backpack** - скин рюкзака. <br>
  **Pants** - скин штанов. <br>
  * __*Значение по умолчанию:*__ <br>
  ```
  "BlockedSkins": {
    "Items": true,
    "Hat": true,
    "Mask": true,
    "Glasses": true,
    "Shirt": true,
    "Vest": true,
    "Backpack": true,
    "Pants": true
  }
  ```
