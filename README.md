# HEditor

HEditor 下面简称 HE ，用于实时调整和预览 H5 游戏的技能，以及其它相关数值编辑，比如物品与合成。

### 为什么要做这个编辑器？

目前市面上游戏相关的编辑器，最强的几个，罗列一下: Flash,DragonBones,Spine,先来说Flash，它是通用的动画编辑器，虽然也有骨骼，但是美术只用传统的关键帧，Flash编辑器无法结合**数值**来预览动画，比如**实时调整**流星雨的下落范围。而后面的两个DragonBones,Spine,也都是专注于人物效果，对于动态的距离和范围控制等等，并不适用。以上三者都只适合制作人物动作和刀光动作。
而实际工作中，除了人物动作和刀光之外，策划还想要实时的预览其它一些战斗效果，如攻击距离，粒子的曲线角度，AOE范围攻击半径，扣血，震屏，声效，打击感等等，还要调整参数后点播放立即生效，而不是输出数据上传再重启游戏，总之，需要有一个工具能完整把控整个技能的节奏，实时的去调整，验证，打磨。
这就是 HE 的应用场合了，将龙骨动画或者帧动画导入进来，再配合节点和数值编辑，实时调整和预览技能。

另外，HE还包含两个重要的功能：物品配置、合成配置。以往的游戏配置，需要策划和程序对 xls 文件进行非常“复杂”的配置，HE 希望能把这种依赖尽量降低，使得游戏的数值配置简单化，并且，HE 希望能在修改数值配置后，能够在编辑器中立即看到变化，比如技能扣血的增减，攻击范围的增减等等。

### HE 到底是什么？
从短期来看，HE 是偏向于数值调整的编辑器（动画调整交给专业的动画编辑器去做），从长期来看 ，HE 将是一个可以深度配置并快速成型的游戏。

### HE 要实现的目标有如下几个：

1. 让技能调制所见即所得（前期）。
1. 支持 buff 的节点式编辑（前期）。
1. 支持导出 JSON 数据让游戏使用（前期）。
1. 支持数值的实时修改（前期）。
1. 支持 buff 等级（后期）。
1. 支持人物动作（dragonbones）和 buff 的回放预览（后期）。
1. 支持简单的AI和副本配置（后期）。
1. 支持物品定义、合成配方定义（而合成这个概念，可以包含并支持升级、强化、奖励，人物、活动等等模块）。（前期）

### 关于HE的几个疑问：

>为什么不直接使用粒子编辑器+配表的方式？
>>因为不直观，不方便实时预览，以至于配表很难做出细致入微的效果（除非操作者非常有耐心并且想象力丰富）。

>为什么不用 starling 或者 html5 来实现界面？
>>因为两者的 input控件 表现不够稳定，同时显存有上限。

>预计支持哪套流程？
>>暂定先支持 Laya 2D，后面如果有时间，加入 Egret 3D支持，或者 three.js。


