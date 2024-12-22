- v1.4.1
    + 修复鼠标移动至已放置的分馏塔时，简洁提示小窗口显示的速率与实际不符的问题。
    + 增产点数对所有分馏塔的影响不再基于加速效果，而是加速效果、增产效果中加成更大的一方。
        + 深空来敌中，有增产调节公理和满增产效果，与无增产调节公理和满加速效果，二者加成是一致的，都为200%。
        + | 增产效果提升 | 加速效果提升 | 公理 | 增产总加成 | 加速总加成 | 分馏加成 |
          |--------|--------|----|-------|-------|------|
          | +0%    | +0%    | ×  | 25%   | 100%  | 100% |
          | +0%    | +0%    | √  | 40%   | 75%   | 160% |
          | +10%   | +100%  | ×  | 35%   | 200%  | 200% |
          | +10%   | +100%  | √  | 50%   | 175%  | 200% |
    + 调整了万物分馏新增的分馏塔，修改部分分馏塔的相关描述。
        + 移除精准分馏塔。
            + 旧存档中已放置的精准分馏塔会自动转换为矿物分馏塔，未知物品2320（原精准分馏塔）需要手动丢弃。
        + 移除建筑极速分馏塔。
        + 不再将原版分馏塔修改为通用分馏塔。
            + 在1.4.1中，原版分馏塔只能用于将氢分馏为重氢，但分馏塔输出优化科技对其依然有效。
            + 在1.4.1中，原版分馏塔无法升降级。如果旧存档启用了创世之书，需要手动拆除所有已建造的原版分馏塔。
        + 添加矿物分馏塔，可分馏所有能直接采集到的矿物（包括氢、水、硫酸、原油等自然资源）。
        + 添加升级分馏塔，可将部分物品转换为更少的高级物品。
        + 添加降级分馏塔，可将部分物品转换为更多的低级物品。
        + 垃圾回收分馏塔优化。
            + 默认禁止输入建筑，以避免误操作。你可以在设置-杂项中开启它。
            + 移除输入物品增产点数的加成。现在，物品转换得到的点数仅与物品价值有关，与是否带有增产点数无关。
            + 调整了电力消耗计算方式，大幅降低处理高价值物品时需要的电力。
        + 点数聚集分馏塔优化。
            + 进一步提升效率，从4%增加至10%。这意味着满带所需建筑数目从25降低到10，占地更小。
            + 优化流动输出物品的增产点数。流动输出平均增产点数不足4时，将输出4点或0点的物品，减少增产剂的消耗。
        + 增产分馏塔优化。
            + 分馏概率不再使用固定值，改为与输入物品的价值有关。价值越高，概率上限就越低。
            + 实际分馏概率与输入物品的增产点数有关。增产点数越多，实际概率越大。0点对应概率0，10点对应概率上限。
    + 降低科技矿物分馏、升降级分馏所需的矩阵数目，以便于前期快速解锁它们。
    + 移除了部分配方，添加了部分矿物自分馏的配方（例如原油、水、硫酸），以符合现在的分馏塔情形。
        + 矩阵分馏链默认关闭。你可以在设置-杂项中开启它。
        + 燃料棒分馏链默认关闭。你可以在设置-杂项中开启它。

- v1.4.0
    + Bug修复
        + 修复黑雾物品未解锁时，仍显示对应分馏配方的问题。
        + 修复普通分馏塔与特殊分馏塔升降级时，产物类型没有正确切换的问题。
        + 修复传送带速度较高时，分馏塔无法满速运行、显示分馏速率错误的问题。
        + 修复分馏塔集装物流科技未显示等级的问题。
        + 修复建筑极速分馏塔显示的速率与实际不符的问题。
        + 修复分馏塔堆叠上限不是30的问题。
    + 调整&优化
        + 【重要】大幅上调增产点数对增产分馏塔的影响。输入10增产点数的物品时，相比之前，产物数目大约变为2.5倍。
        + 【重要】为所有物品添加了1%损毁概率。关闭损毁概率的开关对此次改动同样有效。
        + 拆分图标资源包，修改加载图标的逻辑，现在可以在信号选择页面找到所有的分馏配方图标了。
        + 为部分分馏塔解锁科技添加一定数目的对应的分馏塔作为科技研究奖励。
        + 调整了部分分馏塔的制作配方与HP。
        + 修复拖动分馏详情窗口时，分馏概率字体显示位置错误的问题。
        + 优化分馏配方概率描述。
            + 分馏配方描述中部分数目、概率增加黄色、红色显示，更容易确认分馏配方中特殊的部分。
            + 调整了损毁的描述方式，使其更易于理解。
            + 调整了最下方分馏制作公式的显示，使其与对应分馏配方的概率描述保持一致。
        + 修改特殊分馏塔的处理逻辑，从而大幅提高游戏性能。特殊分馏塔提升80%以上游戏性能。
        + 优化点数聚集分馏塔的处理逻辑，运行效果与之前一致，但概率曲线更为平滑。
        + 【重要】调整所有分馏塔的耗电情况。
            + 垃圾回收分馏塔的耗电与输入的原材点数成正比。分馏详情窗口中左侧输入数目表示原材总点数。
            + 输入物品的增产点数不再影响点数聚集分馏塔的耗电。
            + 输入物品的增产点数对增产分馏塔的耗电影响减半。
            + 启用创世之书时，堆叠对分馏塔耗电影响减半。
        + 适配更多巨构v1.5.0，移除巨构建造页之前的接收器配方，调整所有巨构火箭分馏配方的位置。
        + 调整了创世之书防御页面的大部分图标位置，避免冲突。
    + 新增内容
        + 将所有分馏物品的快捷选择更改为类似巨构的双行选择模式，不再占用原有快捷栏位置。
        + 【重要】新增垃圾回收分馏塔，可以将任意物品转换为沙土或随机物品。
            + 垃圾回收分馏塔的所有接口都可输入，但只有正面的接口能够输出。
            + 如果正面接口未连接，或正面接口不是输出，它将会把所有输入转换为沙土。
            + 如果正面接口是输出，它将会尽可能把输入转换为地基。如果地基数目达到上限，则剩余输入会转换为沙土。
        + 添加精准分馏塔、建筑极速分馏塔、垃圾回收分馏塔的专属解锁科技。
        + 添加分馏塔产物输出集装科技，可以使产物以4堆叠形式输出。所有分馏塔提升10%游戏性能。该科技对精准分馏塔无效。
    + Bug Fixes
        + Fixed the issue that when Black Mist items were not unlocked, the corresponding fractionation recipe was still
          displayed.
        + Fixed the issue that the product type was not switched correctly when normal fractionator and special
          fractionator were leveled up or down.
        + Fixed the issue that when the conveyor belt speed is high, the fractionator cannot run at full speed and the
          fractionation rate is displayed incorrectly.
        + Fixed the issue that the level of fractionator assembly and logistics technology is not displayed.
        + Fix an issue where the displayed rate of Building-HighSpeed Fractionator does not match the actual rate.
        + Fix issue with fractionator stacking cap not being 30.
    + Adjustments & Optimizations
        + [IMPORTANT] Significantly upgraded the effect of proliferator points on Increase Production Fractionators.
          When entering items with 10 proliferator points, the number of products becomes approximately 2.5 times higher
          compared to before.
        + [IMPORTANT] Added 1% destruction probability to all items. The switch to turn off the probability of
          destruction also works for this change.
        + Split the icon resource pack and modified the logic for loading icons, now you can find all fractionation
          recipe icons on the signal selection page.
        + Added a certain number of corresponding fractionators as a tech research bonus for some fractionator unlock
          techs.
        + Adjusted the crafting recipes and HP for some fractionators.
        + Fixed the issue that the Fractionation Probability font was displayed in the wrong position when dragging the
          Fractionation Details window.
        + Optimized fractionation recipe probability descriptions.
            + Added yellow and red color display for number of parts and probability in the description of fractionation
              recipes, making it easier to identify special parts of fractionation recipes.
            + Adjusted the description of damage to make it easier to understand.
            + Adjusted the display of the fractionation crafting formula at the bottom to be consistent with the
              probability description of the corresponding fractionation recipe.
        + Modified the processing logic for special fractionators, resulting in a significant increase in game
          performance. Special fractionators improve game performance by more than 80%.
        + Optimizing the processing logic for the Points Aggregate Fractionator runs as before, but with a smoother
          probability profile.
        + [IMPORTANT] Adjusted power consumption of all fractionators.
            + The power consumption of the Trash Recycle Fractionator is proportional to the number of raw material
              points entered. The number of inputs on the left in the Fractionation Details window represents the total
              number of raw material points.
            + Inputting item's Increase Production Fractionator points no longer affects the power consumption of Points
              Aggregate Fractionator.
            + The effect of inputting items' proliferator points on the power consumption of the Increase Production
              Fractionator is halved.
            + When Book of Creation is enabled, stacking halves the effect on fractionator power consumption.
        + Adapted more megastructures for v1.5.0, removed receiver recipes before the megastructure build page, and
          adjusted the placement of all megastructure rocket fractionation recipes.
        + Adjusted the position of most icons on the Book of Genesis defense page to avoid conflicts.
    + New additions
        + Changed the shortcut selection of all fractionated items to a two-line selection mode similar to the Mega
          Construct, which no longer occupies the original shortcut bar position.
        + [IMPORTANT] Added Trash Recycling Fractionator, which can convert any item into sand or random items.
            + All ports of the Trash Recycling Fractionator can be input, but only the front port can be output.
            + If the front interface is not connected, or if the front interface is not an output, it will convert all
              inputs to sand and earth.
            + If the front interface is an output, it will convert the inputs to foundations if possible. If the number
              of foundations reaches the upper limit, the remaining inputs will be converted to sand.
        + Added exclusive unlockable techs for Precision Fractionator, Building-HighSpeed Fractionator, and Trash
          Recycling Fractionator.
        + Adds the Fractionator Product Output Setting tech, which allows products to be output in stacks of 4. All
          fractionators boost game performance by 10%. This tech does not work on Precision Fractionators.

- v1.3.6
    + 修复了损毁分馏在关闭时仍然生效的问题。
    + Fixed an issue where EnableDestroy was still in effect when it was turned off.

- v1.3.5
    + 修复了未添加创世之书时，mod会导致无法进入游戏的问题。
    + Fixed an issue where the mod would cause the game to be inaccessible when Genesis Book was not added.

- v1.3.4
    + 更改设置后，无需重启游戏，只要重新载入存档即可应用修改。
    + 修改了原版重氢分馏配方。
        + 制作了另外两个样式的图标。
        + 配方描述结尾添加概率说明。
        + 移动配方位置到分馏I。
    + 现已适配创世之书内置的量化工具。
        + 增加两个新的增产策略：加速10点、增产10点。
        + 可以选择分馏配方作为合成路线了。
        + 右键点击工厂，可以将建筑切换为增产分馏塔。
        + 选择的物品配方存在递归时，会在“原料需求”添加额外需要的物品以避免递归计算。
        + 分馏所需建筑的数目与传送带速率有关，计算时强制使用传送带MK3且4堆叠的速率，建筑数目仅供参考。
    + After changing the settings, there is no need to restart the game, just reload the save to apply changes.
    + Modified the original Deuterium Fractionation recipe.
        + Added other two icon styles.
        + Added probability note at end of recipe description.
        + Moved recipe grid index to Fractionate I.
    + Adapted the quantization tool built into Genesis Book.
        + Added two new yield increase strategies: 10 points of acceleration and 10 points of yield increase.
        + Can now select Fractionation recipes as synthesis routes.
        + Right-clicking on a factory switches the building to an Increase Production Fractionator.
        + If the selected recipe is recursive, additional items will be added to the "Raw Material Requirements" to
          avoid recursive calculations.
        + The number of buildings needed for Fractionation is related to the conveyor belt rate, the calculation is
          forced to use the conveyor belt MK3 and 4 stacking rate, the number of buildings is for reference only.

- v1.3.3
    + 载入存档时判断科技解锁状态， 并解锁未解锁的配方。
      这有助于解决为现有存档添加万物分馏时，导致部分分馏建筑、分馏配方未能正确解锁的问题。
    + 修复了新增的分馏塔在传送带上流动时，图标未能正确显示的问题。
    + 优化了使用分馏塔时的统计信息。
        + 点数聚集分馏塔不再添加生产、消耗信息。
        + 增产分馏塔仅添加增加物品的生产信息。
    + 调整部分翻译。
    + 调整了README.md的内容，添加了对应的图片。
    + 使用新的mod介绍图标。
    + Determine technology unlock status when loading an archive and unlock unlocked recipes.
      This helps to solve the problem of adding Fractionate Everything to an existing archive, which causes some
      fractionators and fractionate recipes to not unlock correctly.
    + Fixed an issue where the icon for the new fractionator was not displayed correctly when it was flowing on the
      conveyor belt.
    + Optimized statistics when using fractionators.
        + Points Aggregate Fractionator no longer adds production and consumption information.
        + Increase Production Fractionator only adds production information for increasing items.
    + Adjusted some translations.
    + Adjusted the content of README.md and added corresponding images.
    + Use new mod introduction icon.

- v1.3.2
    + 修复了氢分馏重氢会报错的问题。
    + 修复了切换查看分馏塔时，可能会报错的问题。
    + 修复了分馏塔详情界面中，分馏塔名称没有完全显示的问题。
    + 为重氢分馏配方增加概率描述。
    + 调整了README.md的内容，使其与模组现有内容一致。
    + 调整了加载后弹窗的按钮位置。
    + Fixed an issue where hydrogen fractionate to deuterium would report an error.
    + Fixed an issue where an error could be reported when switching to view fractionators.
    + Fixed an issue where fractionator names were not fully displayed in the fractionator details screen.
    + Added probability description for deuterium fractionation recipes.
    + Adjusted the content of README.md to match the existing content of the module.
    + Adjusted the button position of the popup window after loading.

- v1.3.1
    + 原版增加分馏配方155个；创世之书、更多巨构、深空来袭同时启用时，增加分馏配方217个。
    + 新增首次加载的弹窗，并提供了跳转创世之书交流群、打开更新日志的功能。
    + 为点数聚集分馏塔、增产分馏塔添加了概率说明，并调整了处理逻辑与概率显示。
        + 对于增产分馏塔，如果输入具有自增值分馏配方，将使用该配方概率进行增产；否则使用默认概率。
        + 对于点数聚集分馏塔，输入物品种类不会影响其效果。优化了概率显示。
    + 将所有分馏塔放在同一个升级链中，现在可以使用升降级自由切换分馏塔类型了。
    + 调整部分翻译。
    + 调整部分物品、配方的位置，调整了部分分馏配方。
        + 添加微型粒子对撞机的自分馏配方。
        + 将创世之书部分物品位置改为与配方一致。
        + 调整了创世之书黑雾物品位置、黑雾物品分馏配方位置。
        + 将创世的玻璃改为循环分馏（相当于增加一个分馏配方）。
        + 为创世之书的巨构建筑添加了循环分馏链，但是没有循环链尾加成。
        + 为创世之书添加高斯机枪塔、导弹防御塔的自分馏配方。
        + 调整了更多巨构中运载火箭的分馏顺序，使其符合科技顺序。
    + 配置文件优化。
        + 移除是否显示分馏图标的开关，添加关闭首次加载弹窗的开关。
        + 现在，除了手动修改配置文件，你也可以在游戏的设置页面修改所有配置。
    + 修复大量bug。
        + 修复语言非中文时，矿脉等显示为中文的问题。
        + 修复精准分馏塔、通用分馏塔前置科技异常，从而导致无法制作这些建筑的问题。
            + 启用创世之书时，通用分馏塔的前置科技描述也随之修改。
        + 修复更多巨构中巨构接收器图标重置、效果丢失的问题。
        + 修复创世之书中导弹防御塔配方隐藏的问题。
    + Added 155 fractionation recipes to the original version; 217 fractionation recipes when Genesis Book, More Mega
      Structure, and They Come From Void are enabled at the same time.
    + Added a popup window for the first load, and provided the ability to jump to the Genesis Book exchange group
      and open the update log.
    + Added probability description for Points Aggregate Fractionator and Increase Production Fractionator, and adjusted
      processing logic and probability display.
        + For Increase Production Fractionator, if the input has a self-value-added fractionation recipe, the
          probability of the recipe will be used to increase production; otherwise, the default probability will be
          used.
        + For Points Aggregate Fractionators, entering the item type will not affect its effect. Optimized probability
          display.
    + Putting all fractionators in the same upgrade chain now allows you to freely switch fractionator types using
      elevation.
    + Adjusted some translations.
    + Adjusted the location of some items and recipes, and adjusted some fractionation recipes.
        + Added self-fractionation recipe for Micro Particle Collider.
        + Changed the location of some items in the Genesis Book to match the recipe.
        + Adjusted Genesis Book Dark Fog item locations, Dark Fog item fractionation recipe locations.
        + Changed Genesis' glass to circular fractionation (equivalent to adding a fractionation recipe).
        + Added cyclic fractionation chain to Genesis Book' megastructure building, but without the cyclic chain tail
          bonus.
        + Added self-fractionation recipes for Gauss Machine Gun Towers and Missile Defense Towers to the Book of
          Genesis.
        + Adjusted the fractionation order of carrier rockets in More Mega Structure to match the tech order.
    + Configuration file optimization.
        + Removed the switch for whether to show the fractionation icon, and added a switch to turn off the first load
          popup.
        + You can now change all configurations from the game's settings page, in addition to manually changing the
          config files.
    + Fix a lot of bugs.
        + Fixed the problem that veins etc. are displayed in Chinese when the language is not Chinese.
        + Fix an issue where Precision Fractionator and Universal Fractionator had abnormal technology in front of them,
          which prevented them from crafting these buildings.
            + Fixed an issue where Universal Fractionator's tech description was changed when the Book of Creation was
              enabled.
        + Fixed an issue where the Mega Structure Receiver icon was reset and the effect was lost in More Mega
          Structures.
        + Fix an issue where the Missile Defense Tower recipe was hidden in the Genesis Book.

- v1.3.0
    + 适配创世之书、深空来敌、更多巨构。
        + 这些MOD全部启用时，新增配方个数将超过200。
        + 新的配方同样具有三种样式可供选择。
        + 当同时启用创世之书与万物分馏时，将会使用创世独有材料制作分馏塔。
    + 配置文件优化。
        + 移除配置文件中的配方起始ID，现在会自动使用不重复的配方ID。
        + 添加了自动清除配置文件中无用项目的功能。
    + 现在对于任意速率的传送带，分馏塔都可以满速输出了（之前最大速率为30/s）。
    + 优化了分馏塔界面的分馏成功率显示。
        + 分馏成功率从单行改为多行，可以清晰看到所有概率了。
        + 将“F/D”替换为“流动/损毁”。
    + 调整了部分分馏配方。
        + 提升增产剂分馏配方的产物数目（1,1% -> 2,1%），可以更快产出大量增产剂了。
        + 现在所有循环分馏链的最后一个分馏配方（即分馏链尾变分馏链头）将根据分馏链长度提升物品数目。
    + Adapts Genesis Book, They Come From Void, and More Mega Structure.
        + When all of these mods are enabled, the number of new recipes will be over 200.
        + New recipes are also available in three styles.
        + When both Genesis Book and Fractionation of Everything are enabled, fractionators will be crafted using
          materials unique to Genesis.
    + Config file optimization.
        + Removed recipe start IDs from profiles, now automatically uses non-repeating recipe IDs.
        + Added automatic clearing of useless items from config files.
    + The fractionator can now output at full speed for any rate of conveyor (previously the maximum rate was 30/s).
    + Optimized the display of fractionation success rate in the fractionator interface.
        + Fractionation success rate has been changed from single line to multiple lines, so that all probabilities can
          be clearly seen.
        + Replaced "F/D" with "Flow/Destroy".
    + Adjusted some fractionation recipes.
        + Upgraded the number of products for the Enhancer Fractionation recipe (1,1% -> 2,1%), so that you can produce
          large amounts of Enhancers much faster.
        + The last fractionation recipe of all circular fractionation chains (i.e. the end of the fractionation chain
          becomes the head of the fractionation chain) will now boost the number of items based on the length of the
          fractionation chain.

- v1.2.2
    + 精准分馏塔（原名低功率分馏塔）效果改为缓存的产物越多，分馏效率越低。
    + 新增点数聚集分馏塔，可以将输入物品的增产点数聚集到几个物品上，从而得到10点增产点数的物品。前置科技为新增科技“增产点数聚集”。
    + 增产分馏塔（原名增殖分馏塔）去除本身的10%加成。前置科技为新增隐藏科技“增产分馏”。
    + 点数聚集分馏塔、增产分馏塔可以接受任意物品，无需配方，且产物与输入一致。这次真的万物皆可分馏了！
    + 各种分馏塔现在具有不同的颜色（图标也是如此），可以轻松区分它们了。
    + 新增科技“分馏塔产物集装物流”，研究后，所有分馏塔的产物将以集装形式输出。
    + 增添、移除、调整了部分配方。将所有矩阵分馏配方概率改为1%1个，3%损毁（可以在设置中禁用损毁）。
    + 为所有分馏配方新增了斜线样式、圆弧样式图标。你可以在配置文件中选择三种图标风格之一。
    + 调整了分馏塔的概率显示内容，现在可以准确显示实际的分馏效果。
    + 调整了分馏塔的概率显示刷新频率，从1帧一次减慢至20帧一次，以便清晰看到概率（不会影响建筑处理速率）。
    + The effect of the Precision Fractionator (formerly known as the Low Power Fractionator) has been changed to be
      less efficient at fractionation the more product is cached.
    + Added Points Aggregate Fractionator, which allows you to aggregate the input item's Production Increase Points to
      several items, resulting in a 10 Point Production Increase item. The pre-requisite technology is the new “Yield
      Gathering” technology.
    + Increase Production Fractionator (formerly Increase Production Fractionator) removes its 10% bonus. The new Hidden
      Technology “Fractionation” has been added as a Pre-Tech.
    + Points Aggregate Fractionator and Increase Production Fractionator can accept any item without a recipe, and the
      product is the same as the input. Everything can be fractionated this time!
    + The various fractionators now have different colors (and icons as well), making it easy to tell them apart.
    + Added a new tech called “Fractionator Product Collector Logistics”, which will allow all fractionator products to
      be exported in a collector form.
    + Added, removed, and adjusted some recipes. Changed the probability of all matrix fractionation recipes to 1% for
      1, 3% for destruction (destruction can be disabled in settings).
    + Added new slash style, arc style icons for all fractionation recipes. You can choose one of the three icon styles
      in the config file.
    + Adjusted the probability display content for fractionators, which now accurately displays the actual fractionation
      effect.
    + Adjusted the probability display refresh frequency for fractionators, slowing it down from 1 frame at a time to 20
      frames at a time, so that the probabilities can be seen clearly (without affecting the building processing rate).

- v1.2.0
    + 调整了绝大多数配方的分馏路线！目前新增分馏配方共计155个。其中包括分馏循环链、矿物自分馏等。
    + 为所有分馏配方增加了概率显示。你可以在制作页面查看它们的分馏概率。
    + 将所有配方的图标替换为类似重氢分馏的样式。
    + 物品制作路径中可以看到相关分馏配方了。
    + 修复了解锁科技时，新的分馏配方无法立刻使用的问题。
    + 移除了配置文件中的调整分馏成功率的选项，基础分馏成功率强制使用1%。
    + 原版分馏塔改名为通用分馏塔，建筑效果不变。
    + 增加低功率分馏塔，耗电量变为1/5，分馏成功率变为1/3。
    + 增加建筑极速分馏塔，输入建筑时有12.5%概率分馏成功，否则仅有0.1%概率分馏成功。
    + 增加增殖分馏塔，每次分馏成功有10%概率将输出物品数目翻倍，且增产点数视为增产而非加速。
    + Adjusted the fractionation routes for the vast majority of recipes! A total of 155 new fractionation recipes have
      now been added. These include Fractionation Cycle Chain, Mineral Self-Fractionation, and more.
    + Added probability display for all fractionation recipes. You can view their fractionation probabilities on the
      crafting page.
    + Replaced the icons for all recipes with a style similar to deuterium fractionation.
    + Related fractionation recipes are now visible in the item crafting path.
    + Fixed an issue where new fractionation recipes were not immediately available when unlocking tech.
    + Removed the option to adjust the fractionation success rate in the config file, and forced the base fractionation
      success rate to be 1%.
    + Original Fractionation Tower renamed to Universal Fractionator, building effect remains unchanged.
    + Add low power fractionation tower, power consumption becomes 1/5, fractionation success rate becomes 1/3.
    + Add Building-HighSpeed Fractionator, 12.5% probability of fractionation success when building is entered,
      otherwise only 0.1% probability of fractionation success.
    + Add Augmentation fractionator, each successful fractionation has a 10% chance of doubling the number of output
      items, and augmentation points are treated as augmentation instead of acceleration.

- v1.1.0
    + 适配版本 0.10.29.22015。
    + 新增了1个分馏配方，目前新增分馏配方共计105个。
    + 为每个分馏配方添加了图标显示，图标为产物图标。
    + 为每个分馏配方添加了前置科技，解锁科技将会同步解锁相应的分馏配方。
    + 允许自定义是否启用前置科技。如果不启用，所有分馏配方将在开局可用。
    + 允许自定义是否显示所有的分馏配方。
    + 允许自定义从哪一页开始显示新的分馏配方（用于避免mod之间可能存在的配方显示冲突）。
    + 允许自定义从哪个ID开始添加分馏配方（用于避免mod之间可能存在的配方ID冲突）。
    + Updated to work with game version 0.10.29.22015.
    + 1 new fractionation recipe has been added, for a current total of 105 new fractionation recipes.
    + Pre-techs have been added for each fractionation recipe, and unlocking a tech will unlock the corresponding
      fractionation recipe at the same time.
    + Allows customization of whether previous technology is enabled. If not enabled, all fractionation recipes will be
      available at the beginning.
    + Add icon display for each fractionated recipe.
    + Allow customization of whether all fractionated recipes are displayed.
    + Allow to customize from which page new fractionated recipes are displayed (used to avoid possible recipe display
      conflicts between mods).
    + Allow to customize from which ID to start adding fractionated recipes (used to avoid possible recipe ID conflicts
      between mods).

- v1.0.1
    + 适配版本 0.10.29.21950。
    + 新增了3个分馏配方，目前新增分馏配方共计104个。
    + Updated to work with game version 0.10.29.21950.
    + 3 new fractionation recipes has been added, for a current total of 105 new fractionation recipes.

- v1.0.0
    + 适配版本 0.10.28.21014。
    + 新增了一些分馏配方，包括新的武器、物品等。目前新增分馏配方共计101个。
    + Updated to work with game version 0.10.28.21014.
    + Add some fractionate recipes with new buildings and items. A total of 101 new fractionation recipes have now been
      added.
