# ChatManager

* Chats
  * __*Тип данных:*__ ```List<Chat>```
  * __*Описание:*__ <br> Type - тип чата, который требуется настроить. (```string ("GLOBAL"/"GROUP"/"LOCAL")```)<br>
  Block - нужно ли блокировать чат или нет. (```bool```)<br>
  AdminByPass - обходят ли "синие" админы блокировку чата. (```bool```)<br>
  ByPassPermission - разрешение на обход блокировки чата. (```string```)<br>
  ShouldRedirect - перенаправляет ли плагин сообщение игрока в другой чат, если текущий чат заблокирован. (```bool```)<br>
  RedirectTo - в какой чат перенаправить сообщение игрок. (```string ("GLOBAL"/"GROUP"/"LOCAL")```)
  * __*Значение по умолчанию:*__ <br> 
 ```
[
    {
      "Type": "GLOBAL",
      "Block": true,
      "AdminByPass": true,
      "ByPassPermission": "DI.GlobalChatByPass",
      "ShouldRedirect": true,
      "RedirectTo": "LOCAL"
    },
    {
      "Type": "GROUP",
      "Block": true,
      "AdminByPass": true,
      "ByPassPermission": "DI.GroupChatByPass",
      "ShouldRedirect": false,
      "RedirectTo": "LOCAL"
    },
    {
      "Type": "LOCAL",
      "Block": false,
      "AdminByPass": false,
      "ByPassPermission": null,
      "ShouldRedirect": false,
      "RedirectTo": "LOCAL"
    }
]
```
