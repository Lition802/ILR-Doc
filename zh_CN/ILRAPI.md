## RunnerAPI

```luaapi:createEntityObject(intptr:playerintptr)```

```luaapi:createPlayerObject(string:uuid)```

 - 从实体指针创建可操作对象
 
```lua
i = mc:createEntityObject(intptr)
print(i.ArmorContainer) --玩家装备栏
print(i.Attack) --玩家攻击力
print(i.Attributes) --实体属性表
print(i.CollisionBox) --碰撞箱
print(i.DimensionId) --实体维度
print(i.Effects) --实体所有状态效果表
print(i.HandContainer) --主副手栏
print(i.Health) --生命值
print(i.HotbarContainer) --玩家热键栏
print(i.InventoryContainer) --背包列表
print(i.MaxAttributes) --实体属性最大值表
print(i.Position) --实体坐标
print(i.Rotation) --实体转角属性
print(i.TypeId) --实体类型ID
print(i.UniqueId) --查询ID
print(i.Uuid) --UUID
print(i:getName()) --实体名字
i:setName(string:name,bool:ifalways) --重命名，True为是否一直显示
i:addLevel(int:level) --给予玩家等级
i.remove --从地图清除实体
```

```luaapi:Listen(string:key,function:func)```

 - 把一个函数放到监听器列表
 - 注意：key不对会注册失败
 
```luaapi:teleport(string:uuid,int:x,int:y,int:z,int:did)```

 - Hook内容需要随版本更新

```luaapi:GetXUID(string:playername)```

- 从玩家名查询xuid
- 查询失败返回nil

```luaapi:GetUUID(string:playername)```

- 从玩家名查询uuid
- 查询失败返回nil
