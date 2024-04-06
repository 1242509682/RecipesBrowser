## 插件说明
```
版本: 0.5  
作者：棱镜  
适配：羽学  
源发布地址：https://www.bbstr.net/t/598/  
开源地址：https://github.com/1242509682/RecipesBrowser

由于PE的Terraria的向导存在一些恶性bug，  
导致在大多数服务器中向导被禁用，这样一来想要查合成表就非常麻烦，  
所以写了这样一个插件，支持查找“此物品的配方”和“此物品可以合成什么”
```
## 命令
```
可用指令：/查、/fd、find
查合成铜短剑需要什么材料：/fd 铜短剑
查铜短剑可合成什么物品：/fd 铜短剑 r
```

## 权限
```
RecipesBrowser  
在Tshock控制台发送这个，给玩家添加权限：/group addperm default RecipesBrowser 
```

## 更新日志
修复了0.4版没有释放资源导致的以下错误：
```(C#)
Stack overflow.
Repeat 130877 times:
--------------------------------
   at TerrariaApi.Server.TerrariaPlugin.Dispose()
   at MainPlugin.Dispose(Boolean)
--------------------------------
   at TerrariaApi.Server.ServerApi.UnloadPlugins()
   at TerrariaApi.Server.ServerApi.DeInitialize()
   at TerrariaApi.Server.Program.Main(System.String[])
   at Program+<>c__DisplayClass0_0.<<Main>$>g__Start|1()
   at Program+<<Main>$>d__0.MoveNext()
   at System.Runtime.CompilerServices.AsyncMethodBuilderCore.Start[[Program+<<Main>$>d__0, TShock.Server, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null]](<<Main>$>d__0 ByRef)
   at System.Runtime.CompilerServices.AsyncTaskMethodBuilder.Start[[Program+<<Main>$>d__0, TShock.Server, Version=1.0.0.0, Culture=neutral, PublicKeyToken=null]](<<Main>$>d__0 ByRef)
   at Program.<Main>$(System.String[])
   at Program.<Main>(System.String[])
Aborted (core dumped)
```
