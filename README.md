# xyn军火库之CoyoteSix：读取彩虹六号游戏内死亡信息等实时数据，改变郊狼强度

Edit: This project is currently not actively managed. Please read my code, understand the logic, and write your own implementation.

更新：这个项目不维护了，请自己读我的代码来写你自己的更新。

Please note that Ubisoft does not offer any API for real-time in-game stats.

育碧官方没有提供任何可以读取游戏内实时数据的API。

You can try applying for a R6 Tracker developer account. R6 Tracker, which is greenlit by Ubisoft, offers such APIs but the application process is very strict and tedious.

R6 Tracker有提供这样的API，你可以申请开发者账号，但过程非常严格和麻烦。

## A Simple Explanation

xyn军火库+1。大概就是通过OBS读取屏幕上的像素点来判断生存、死亡、游戏结束。育碧没给API，但你也别问我为什么不用Vulkan/DX11/DX12缓冲区，一是我不会，二是Vulkan被狗日的育碧移除了，三是性能问题，四是你号不想要了是吧？你tm干脆直接读内存算了，举头三尺有神明，BattlEye都看着呢！这都得应验的。————习近平

Basically, it determines survival, death, and game over by reading the pixels on the screen through OBS. Don’t ask me why I don’t use Vulkan/DX11/DX12 buffers—first, I don’t know how; second, Vulkan was damn removed by Ubisoft; third, performance issues; fourth, you wanna get your account banned or what? Might as well read memory directly, right? BattlEye is watching you bro
