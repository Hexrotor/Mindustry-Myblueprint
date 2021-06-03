# Mindustry-Myblueprint
萌新个人制作蓝图和逻辑，仅适用于战役。未照搬他人作品，如有雷同纯属雷同，欢迎体验！<br>
**注意，我的游戏版本为126.2**<br>

### 雷霆敢死队1.2
控制雷霆自动从核心拿爆混后轰炸敌方炮塔或核心，并在低于一定生命值时自动返回核心。自动携带地面单位(最多4个，但跟随模式不受限制)，自动攻击地面敌人。附近有敌人(包括空军)自动释放单位，低生命值返回核心时自动释放单位，关闭携带开关时释放所有单位。单位携带数、最低生命值、携带物、轰炸对象可自定义。<br>
注意：由于代码过多，单位过多时某些功能可能效果不佳；单位携带功能不一定实用，请酌情使用；判断可携带单位使用了血量比对(仅携带900及以下，但跟随模式不受限制)，所以您如果安装了某些模组，这可能会引发问题。<br>

行为优先级：取携带物>跟随玩家=自爆=释放单位>攻击核心>低血量返回>攻击敌人>携带单位>攻击炮塔<br>

按钮的功能：<br>
* 左下为总开关，开启后从核心拿爆混后自动轰炸敌方炮塔，并在低于一定生命值时返回。若低于设定的自爆生命值，则会冲向敌方炮塔直到爆炸。<br>
* 左上为轰炸核心开关，开启后会直接拿爆混冲向敌方核心，不会返回。此开关比右上玩家操控开关优先级低，但此开关开启时影响玩家操控模式时的低血量返回程序，即低血量不会返回。<br>
* 右上为跟随玩家开关，开启后会覆盖轰炸核心的命令，优先跟随玩家。此开关开启时，玩家可以通过操控"电弧"来控制单位移动，玩家可带2~3个雷霆绕到敌方核心，并在接近时关闭并切换到轰炸核心命令。<br>
* 顶部为单位携带开关，开启后自动携带附近陆军，关闭后释放所有单位。<br>
* 分类器可以选择携带物，默认为爆混。<br>

**没有调用冲突检测！**<br>

[预览](https://cdn.jsdelivr.net/gh/Hexrotor/Mindustry-Myblueprint/boom1.2.jpg)
[获取](https://cdn.jsdelivr.net/gh/Hexrotor/Mindustry-Myblueprint/boom1.2.txt)<br>

### 煤站改
修改后的煤站，装弹效率有点低，但增加了库存。<br>
[预览](https://cdn.jsdelivr.net/gh/Hexrotor/Mindustry-Myblueprint/coal2.png)
[获取](https://cdn.jsdelivr.net/gh/Hexrotor/Mindustry-Myblueprint/coal2.txt)<br>

### 陆辅T1~T4自动跟随玩家
通过电弧操控单位前往指定坐标攻击或跟随玩家攻击。玩家未控制时自动攻击敌人，但不会攻击敌方建筑。注意不要进入石油、深水区域。<br>

**没有调用冲突检测！**<br>

[预览](https://cdn.jsdelivr.net/gh/Hexrotor/Mindustry-Myblueprint/followplayer.jpg)
[获取](https://cdn.jsdelivr.net/gh/Hexrotor/Mindustry-Myblueprint/followplayer.txt)<br>

### T3&T4红飞机控制
通过电弧操控T3&T4红飞机单位前往指定坐标攻击。若玩家不控制，则自动锁定并攻击附近敌人。锁定后可远程追踪，需要手动操作才能切换锁定对象。<br>

**没有调用冲突检测！**<br>

[预览](https://cdn.jsdelivr.net/gh/Hexrotor/Mindustry-Myblueprint/airctrl.jpg)
[获取](https://cdn.jsdelivr.net/gh/Hexrotor/Mindustry-Myblueprint/airctrl.txt)<br>

### Mega自动采矿+攻击闪避
自动开采核心内最少的物品(铜铅煤钛)同时保留自动修复，可手动选择开采物，扣血量超过10自动返回基地。优先攻击敌人，并反复横跳躲避攻击。对于无钛的地图可能会出问题，稍加修改数量判定代码即可。<br>

**没有调用冲突检测！众所周知煤是易燃物，进入核心有风险，故推荐使用挖矿选择器。**<br>

[预览](https://cdn.jsdelivr.net/gh/Hexrotor/Mindustry-Myblueprint/megaplus.jpg)
[获取](https://cdn.jsdelivr.net/gh/Hexrotor/Mindustry-Myblueprint/megaplus.txt)<br>

### 幻型自动修复(不推荐)
抓取一个Poly单位自动修复受损结构，修复完成后停留在基地。也许对于前期有用？<br>

**没有调用冲突检测！没有敌人规避功能且approach半径为1，经测试效果不佳。**<br>

[预览](https://cdn.jsdelivr.net/gh/Hexrotor/Mindustry-Myblueprint/polyrepair.jpg)
[获取](https://cdn.jsdelivr.net/gh/Hexrotor/Mindustry-Myblueprint/polyrepair.txt)<br>

### 钍炸弹
利用爆炸的钍堆消灭周围的一切。自动调用星辉或独影装填钍，钍堆生命值低于500自动引爆，可手动引爆。<br>
按钮的功能：左侧按钮解除热量限制，即引爆；右侧按钮选择调用星辉或独影，默认为星辉。<br>

**仅调用闲置的单位，调用的单位会被赋予随机flag值以供其余处理器区分，结束后恢复flag值为0。当心您的支援单位被误伤！**<br>

[预览](https://cdn.jsdelivr.net/gh/Hexrotor/Mindustry-Myblueprint/autoboom.jpg)
[获取](https://cdn.jsdelivr.net/gh/Hexrotor/Mindustry-Myblueprint/autoboom.txt)<br>

### 独影仓库搬运
显示物品统计并当仓库单物品容量仅剩50时控制独影将物品搬运到核心。需要手动链接仓库(一对一)，并在代码内设置仓库名称。<br>

**调用单位可自行修改，仅调用闲置的单位，调用的单位会被赋予同一随机flag值以供其余处理器区分。由于技术原因flag值不会恢复，但不影响本逻辑的运行。**<br>

[预览](https://cdn.jsdelivr.net/gh/Hexrotor/Mindustry-Myblueprint/monotrans.jpg)
[获取](https://cdn.jsdelivr.net/gh/Hexrotor/Mindustry-Myblueprint/monotrans.txt)<br>

### 石油站
需要外部供应石油(供应点在左下)，可以在有石油的状态下自启动，非常强大。和煤站一样，容易火灾。<br>
[预览](https://cdn.jsdelivr.net/gh/Hexrotor/Mindustry-Myblueprint/petroleum.png)
[获取](https://cdn.jsdelivr.net/gh/Hexrotor/Mindustry-Myblueprint/petroleum.txt)<br>

### 水站
需要大面积的水，局限性很大。<br>
[预览](https://cdn.jsdelivr.net/gh/Hexrotor/Mindustry-Myblueprint/water.png)
[获取](https://cdn.jsdelivr.net/gh/Hexrotor/Mindustry-Myblueprint/water.txt)<br>

### 水站PLUS
需要小面积水，大面积空地。<br>
[预览](https://cdn.jsdelivr.net/gh/Hexrotor/Mindustry-Myblueprint/waterplus.png)
[获取](https://cdn.jsdelivr.net/gh/Hexrotor/Mindustry-Myblueprint/waterplus.txt)<br>

### 钍站
需要放入钍来启动(也可自启动)，启动过程会轻微负电。做成一体式是为了好看，实际操作还是按地形部署比较简便。<br>
[预览](https://cdn.jsdelivr.net/gh/Hexrotor/Mindustry-Myblueprint/tu.png)
[获取](https://cdn.jsdelivr.net/gh/Hexrotor/Mindustry-Myblueprint/tu.txt)<br>
[PLUS预览](https://cdn.jsdelivr.net/gh/Hexrotor/Mindustry-Myblueprint/tuplus.png)
[PLUS获取](https://cdn.jsdelivr.net/gh/Hexrotor/Mindustry-Myblueprint/tuplus.txt)<br>

### 废料冲击
可能需要绿带才能带动，多余物品会被自动销毁，稳定后发电量7.7k左右。<br>
[预览](https://cdn.jsdelivr.net/gh/Hexrotor/Mindustry-Myblueprint/reactor.jpg)
[获取](https://cdn.jsdelivr.net/gh/Hexrotor/Mindustry-Myblueprint/reactor.txt)<br>
