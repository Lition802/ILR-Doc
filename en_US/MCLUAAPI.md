# MCLUAAPI

```mc:listen(string:key,function:fun)```

 -Register a listener
  - If the key is incorrect, registration will fail
 
```mc:runcmd(string:cmd)```

  - Execute background commands

```mc:reNameByUuid(string:uuid,string:name)```

  - Rename the UUID corresponding to the player

```mc:selectPlayer(string:uuid)```

  - Query basic player information corresponding to UUID

```mc:getOnLinePlayers()```

  - Get a list of online players
  - Contains player uuid and xuid information

```mc:getscoreboard(string:uuid,string:objname)```

  - Get uuid corresponding to the value on the player's specific scoreboard
  - If the scoreboard does not exist, it will be created automatically

```mc:setCommandDescribe(string:key,string:describe)```

  - Set a global command description

```mc:sendText(string:uuid,string:msg)```
 
  - Send a text message to the player corresponding to the UUID

```mc:sendSimpleForm(string:uuid,string:title,string:context,string:Array)```

  - Send a normal form to the player corresponding to the UUID
  - Array format: ```["I am the first row", "I am the second row, "I am the third row"]```

```mc:sendModalForm(string:uuid,string:title,string:context,string:botton1,string:botton2)```

  - Send a modal dialog to the player corresponding to the UUID
  - botton1 and botton2 are the text displayed by the button

```mc:sendCustomForm(string:uuid,string:json)```

   -Send a custom form to the player corresponding to the UUID
  - The json format is as follows
``` json
{"content":[{"type":"label","text":"This is a text label"},{"placeholder":"watermark text","default":"","type":" input","text":""},{"default":true,"type":"toggle","text":"switch~maybe it is"},{"min":0.0,"max": 10.0,"step":2.0,"default":3.0,"type":"slider","text":"Cursor slider!?"},{"default":1,"steps":["Step 1 ","Step 2","Step 3"],"type":"step_slider","text":"Matrix slider?!"},{"default":1,"options":["Option 1" ,"Option 2","Option 3"],"type":"dropdown","text":"As you can see, dropdown box"}], "type":"custom_form","title":"this Is a custom form"}
```

```mc:runcmdAs(string:uuid,string:cmd)```

  - Simulate UUID to execute a command corresponding to the player
  - The original command does not need to add /, the plug-in command needs to be added

```mc:disconnectClient(string:uuid,string:tips)```

  - Disconnect the player corresponding to the UUID
  - tips are the tips when disconnecting
  - If the LoadName event is disconnected, there may not be a custom prompt

```mc:addPlayerItem(string:uuid,int:itemid,int:itemaux,int:count)```

  - Add an item for the UUID corresponding player
  - It may not take effect when the player’s backpack is full


```mc:talkAs(string:uuid,string:msg)```

  - Simulate UUID and say a word to the player
