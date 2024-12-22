![](https://s2.loli.net/2024/04/08/LtlNkxZD4jmdbFX.jpg)

> “走自己的路，不要随波逐流。” —— 重氢
>
> "Don't just follow the path. Make your own trail." —— Deuterium

# 万物分馏(Fractionate Everything)

包含5个不同功能的分馏塔，以及超过200个分馏配方。所有分馏配方均会随着科技的进步逐渐解锁。

**_尽情享受分馏的乐趣吧！_**

<details>
<summary>点击此处查看模组详细信息</summary>

## MOD简介

### 不同功能的分馏建筑

![](https://s2.loli.net/2024/05/19/wqcyU5M2QOr3knC.png)

- 精准分馏塔：速率越低，分馏成功率越高。

- 建筑极速分馏塔：输入建筑时，大幅提高分馏成功率；否则大幅降低分馏成功率。

- 通用分馏塔：使用极速传送带且集装货物情况下，速率优于精准分馏塔。

- 点数聚集分馏塔：将增产点数集中到一小部分产品上，达到10点后输出。

- 增产分馏塔：增产剂的效果改为提升物品输出数目，从而达到无中生有。

以上是MOD包含的五种分馏建筑，你可以使用升降级功能在这些建筑之间自由切换。

### 精心设计的分馏配方

![](https://s2.loli.net/2024/05/19/DAlhnkyewYKOS3L.png)

万物分馏的分馏路线经过了仔细考虑，尽量保证游戏的体验。

![](https://s2.loli.net/2024/05/19/Ofr48jBz3m9FeId.png)

原版游戏无论如何分馏，物品整体数目都不会变。万物分馏对分馏配方进行了拓展，使其具有一个原料产出多个产品的能力。同时，如果配方有损毁概率，有可能导致原料消失。

![](https://s2.loli.net/2024/05/19/Q4LgWKT5yAF6wIU.png)

MOD的分馏配方已经过仔细调整，其中包含部分循环链。一些循环链的链尾物品分馏为链头物品的配方具有产物数目加成。矩阵分馏配方包含损毁概率。

![](https://s2.loli.net/2024/05/19/D2QKpiEXCP3lN1r.png)

每个配方都有三种图标样式可供切换，你可以自由选择喜欢的样式。

### 可以适配大多数MOD

![](https://s2.loli.net/2024/05/19/CVzbMQX2F1iDIrR.png)

万物分馏对一部分大型MOD做了适配，为这些MOD添加了独特的分馏配方。

尤其是创世之书的适配，不仅制作了专属分馏路线，还将所有分馏建筑的制作配方改为使用创世独有材料。

推荐与创世之书、更多巨构、深空来袭一同启用。同时启用时，分馏配方的数目将会超过200个。

### 跟随科技逐步解锁

![](https://s2.loli.net/2024/05/19/18I7mBtgDS43VJH.png)

随着科技不断解锁，新的分馏塔、分馏配方也会跟随解锁。注意，增产分馏塔的前置科技为隐藏科技，它会在合适的时间展现。

![](https://s2.loli.net/2024/05/19/JImBbpz5lQHgRKi.png)

除此之外，还增加了分馏塔集装物流科技。该科技对所有分馏塔都生效，可以使分馏塔的产物尽可能以集装形式输出。

## 安装方法

### 使用Mod管理器安装

打开mod管理器（如果你还没安装可以[**点此安装**](https://dsp.thunderstore.io/package/ebkr/r2modman/)），
下载并启用**FractionateEverything**。

### 手动安装

以下使用`%gamepath%`表示游戏目录。假如你通过Steam启动游戏，右键戴森球计划->属性...->已安装文件->浏览...，即可打开游戏目录。

1. 安装 [BepInEx](https://thunderstore.io/c/dyson-sphere-program/p/xiaoye97/BepInEx/) ，将其解压到`%gamepath%`下。
2. 安装 [LDBTool](https://thunderstore.io/c/dyson-sphere-program/p/xiaoye97/LDBTool/)
   和 [CommonAPI](https://thunderstore.io/c/dyson-sphere-program/p/CommonAPI/CommonAPI/)。
3. 将下载的万物分馏压缩包解压至`%gamepath%\BepInEx\plugins`。确保有如下文件：
    * `%gamepath%\BepInEx\plugins\MengLei-FractionateEverything\FractionateEverything.dll`
    * `%gamepath%\BepInEx\plugins\MengLei-FractionateEverything\fracicons`

## 修改配置

### 如何修改配置

配置文件路径：`%gamepath%\BepInEx\config\com.menglei.dsp.FractionateEverything.cfg`

**至少运行过游戏一次**才会出现配置文件。修改后需**重启游戏**才会生效。

你可以直接修改配置文件，或者在游戏的“设置-杂项”里面修改（推荐）。

### 可修改的项目

- DisableMessageBox：是否禁用首次加载时的提示信息。

- IconVersion：使用哪个版本的分馏图标。

  1表示原版重氢分馏样式，2表示直线分割样式，3表示圆弧分割样式。

- EnableDestroy：是否启用分馏配方中的损毁概率。

  启用情况下，有损毁概率的分馏配方（通常为矩阵）分馏时原料有概率损毁（推荐）。

## 致谢

- 特别感谢jinxOAO。该MOD的灵感来源于他的[FractionateUniverse](https://dsp.thunderstore.io/package/jinxOAO/FractionateUniverse/)，没有他的模组就不会有万物分馏。他还帮助我解决了科技解锁时建筑不接受新的分馏配方的问题，提供了一种修改建筑耗电的方法，并指出分馏塔升级意义不大，不如制作新功能的分馏塔。正是如此，现在的分馏塔才拥有不同的功能，而非仅仅是效率上的提升。

- 特别感谢Awbugl。作为创世之书目前的代码编写者，他帮助我解决了MOD编写的绝大多数难点，非常感谢他的无私帮助。并且，万物分馏很多代码逻辑参考了创世之书的代码，例如主页面加载弹窗、与其他MOD进行适配等等，这方便了我的开发。

- 特别感谢L。作为最早一批的测试人员，他的积极测试与鼓励使我拥有坚持完善万物分馏的决心。文档最顶端的[图片](https://s2.loli.net/2024/04/08/LtlNkxZD4jmdbFX.jpg)就是他提供的。

- 特备感谢飞鸿，测试MOD并提供了大量建议。他提供了部分分馏塔的功能想法，并反馈给我矩阵分馏配方的不合理性。分馏损毁功能正是源于他的测试，这个功能大幅提高了MOD的游戏体验。

- 特别感谢创世之书交流群的群友，正是由于他们的不断反馈，我才能修复MOD中存在的问题，并对MOD进行功能上的修改。

- 特别感谢使用万物分馏的每一位玩家，希望你们能感受到分馏的乐趣。如果你有任何错误信息或建议，欢迎加入[创世之书交流群](https://jq.qq.com/?_wv=1027&k=5bnaDEp3)并反馈给我（@萌泪）。

</details>

Includes 5 fractionators with different functions and over 200 fractionate recipes. All fractionate recipes will be
unlocked gradually with the advancement of technology.

**_Have fun with fractionation!_**

<details>
<summary>Click here for mod details</summary>

> Tips: The image below is shown in Chinese, but the mod has been adapted with English translation, so don't worry about it.

## MOD Introduction

### New Fractionators with different functions

![](https://s2.loli.net/2024/05/19/wqcyU5M2QOr3knC.png)

- Precision Fractionator: the lower the rate, the higher the fractionate success rate.

- Building-HighSpeed Fractionator: when inputting a building, the fractionate success rate is dramatically increased;
otherwise, the fractionation success rate is dramatically decreased.

- Universal Fractionator: better rate than Precision Fractionator when using Extreme Conveyor and gathering cargo.

- Points Aggregate Fractionator: Concentrates Increase Production Points on a small percentage of product and outputs them
after reaching 10 points.

- Increase Production Fractionator: the effect of the Increase Production Agent is changed to boost the number of items
output, thus creating something out of nothing.

These are the five types of Fractionators included in the mod, and you can freely switch between these buildings using
the level up and down function.

### Well-designed fractionate recipes

![](https://s2.loli.net/2024/05/19/DAlhnkyewYKOS3L.png)

The fractionate routes of Fractionate Everything have been carefully considered to ensure as much of a gameplay
experience as possible.

![](https://s2.loli.net/2024/05/19/Ofr48jBz3m9FeId.png)

In the original game, the overall number of items remains the same no matter how they are fractionated. Fractionate
Everything has expanded the fractionate recipe to have the ability to produce multiple products from a single
ingredient. Also, if the recipe has a damage probability, it may cause the ingredient to disappear.

![](https://s2.loli.net/2024/05/19/Q4LgWKT5yAF6wIU.png)

The MOD's fractionate recipes have been carefully tweaked to include some of the circular chains. Some recipes for
fractionate end-of-chain items into head-of-chain items have a product count bonus. Matrix fractionate recipes
include damage probability.

![](https://s2.loli.net/2024/05/19/D2QKpiEXCP3lN1r.png)

Each recipe has three icon styles to switch between, so you are free to choose your favorite style.

### Adaptable to most mods

![](https://s2.loli.net/2024/05/19/CVzbMQX2F1iDIrR.png)

Fractionate Everything has been adapted to some of the large mods, adding unique fractionate recipes to these mods.

In particular, Genesis Book adaptation not only made exclusive fractionate routes, but also changed the
crafting recipes for all fractionators to use Genesis-exclusive materials.

It is recommended to enable it together with Genesis Book, More Mega Structure, and They Come From Void. When
enabled at the same time, the number of fractionate recipes will exceed 200.

### Unlocked gradually with technology

![](https://s2.loli.net/2024/05/19/18I7mBtgDS43VJH.png)

As technology is unlocked, new fractionators and fractionate recipes will also be unlocked. Note that the pre-tech for
the Increase Production Fractionator is a hidden tech that will be revealed at the right time.

![](https://s2.loli.net/2024/05/19/JImBbpz5lQHgRKi.png)

In addition to this, the Fractionator Product Integrated Count Logistics tech has been added. This tech is effective for
all fractionators, and allows the products of the fractionator to be exported as much as possible in a cargo.

## Installation

### Install using Mod Manager

Open the mod manager (you can [**click here to install**](https://dsp.thunderstore.io/package/ebkr/r2modman/) if you
haven't already) and
Download and enable **FractionateEverything**.

### Manual installation

The following uses `%gamepath%` to indicate the game directory. Assuming you launched the game via Steam, right-click
Dyson Sphere Program -> Properties... -> Installed Files -> Browse... to open the game directory.

1. Install [BepInEx](https://thunderstore.io/c/dyson-sphere-program/p/xiaoye97/BepInEx/) and extract it
   under `%gamepath%`.
2. Install [LDBTool](https://thunderstore.io/c/dyson-sphere-program/p/xiaoye97/LDBTool/)
   and [CommonAPI](https://thunderstore.io/c/dyson-). sphere-program/p/CommonAPI/CommonAPI/).
3. Extract the downloaded Fractionate Everything zip to `%gamepath%\BepInEx\plugins`. Make sure you have the following
   files:
    * `%gamepath%\BepInEx\plugins\MengLei-FractionateEverything\FractionateEverything.dll`
    * `%gamepath%\BepInEx\plugins\MengLei-FractionateEverything\fracicons`

## Modify the configuration

### How to modify the configuration

Configuration file path: `%gamepath%\BepInEx\config\com.menglei.dsp.FractionateEverything.cfg`

**Run the game at least once** for the config file to appear. You need to **restart the game** after modifying it for it
to take effect.

You can change the configuration file directly, or in the game's “Settings - Miscellaneous” (recommended).

### Modifiable items

- DisableMessageBox: Don't show message when FractionateEverything is loaded.

- IconVersion: Which style of the fractionate recipe icon to use.

  1 for original deuterium fractionate style, 2 for slanting line segmentation style, 3 for circular segmentation style.

- EnableDestroy: Whether to enable the probability of destruction in fractionate recipes.

  When enabled, Fractionation recipes with a probability of destruction (usually matrix) fractionate with a probability
  of destruction of the feedstock (recommended).

## Credits

- Special thanks to jinxOAO. the mod was inspired by
  his [FractionateUniverse](https://dsp.thunderstore.io/package/jinxOAO/FractionateUniverse/), without his module there
  would be no Fractionate Everything. He also helped me solve the problem of buildings not accepting new fractionation
  recipes when tech is unlocked, provided a way to modify the power consumption of buildings, and pointed out that there
  was little point in upgrading fractionator towers, and that it would be better to make fractionators with new
  features. This is exactly why the fractionator now has a different function, not just an efficiency boost.

- Special thanks to Awbugl. as the current coder of the Genesis Book, he has helped me solve most of the difficulties in
  writing the mod, and his selfless help is greatly appreciated. Moreover, many of the code logic of Fractionate
  Everything references the code of Book of Genesis, such as loading pop-up windows on the main page, adapting with
  other mods, etc., which facilitates my development.

- Special thanks to L, as the first batch of testers, his active testing and encouragement make me have the
  determination to insist on perfecting Fractionation. The [image](https://s2.loli.net/2024/04/08/LtlNkxZD4jmdbFX.jpg)
  at the top of the document is provided by him.

- Special thanks to 飞鸿, who tested the MOD and provided tons of advice. He provided some of the ideas for the
  functionality of the fractionator and gave me feedback on the irrationality of the matrix fractionation recipe. The
  Fractionation Damage feature originated from his testing, and this feature drastically improves the gameplay
  experience of the mod.

- Special thanks to the group members of the Genesis Book exchange group, it was thanks to their constant feedback that
  I was able to fix the problems in the mod and make functional changes to the mod.

- Special thanks to every player who uses Fractionate Everything, I hope you have fun with fractionation. If you have any
  bug or idea, please give me feedback on [Github Issue](https://github.com/MengLeiFudge/MLJ_DSPmods/issues/new).

</details>
