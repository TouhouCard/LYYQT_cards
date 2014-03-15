胧月夜绮谭 卡片脚本
============

包括所有卡牌脚本，目前目录排列方式是

卡牌类型/所属人物/卡牌编码/版本.文件类型

卡牌类型
--------

	SC: Spell Card 符卡 (卡背：月)
	CC: Character Card 人物卡 (卡背：胧)
	WC: Weather Card 场地卡 (卡背:夜)
	BA: Back Art 背面图案(无人物和编码信息)(这个还得带特效么喵？)

所属人物
--------

仅针对有人物依存的卡牌，按照人物罗马音拼写命名文件夹

若所属多只，则用 & 符号连接所属人物名字（按照攻受顺序（大雾

若无所属，则用 Free 命名文件夹

	对于 BA 卡牌来说，没有这级目录。

卡牌编码
--------

卡牌发售时候给定的编码

	对于 BA 文件夹，仅存在  LONG / YUE / YE 三个目录

版本
--------

卡牌发售时所给定的版本，比如 EX11.0.1.0 这样。如果是体验版，则版本号为 Alpha/Beta/Demo 等等。

	对于 BA 文件夹，目前仅存在 default 版本文件

文件类型
--------

目前支持三种后缀类型： js/coffee/json 

	注意：脚本搜索顺序是  js -> coffee -> json, .coffee 可以被预编译为 .js 文件。

文件格式
--------

以 CoffeeScript 为基准，每个文件最终导出一个 class 来描述卡牌的各个信息。