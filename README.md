# 全国383个城市历史空气质量数据及代码
尝试使用selenium对全国383个城市2013年末至2018年8月空气质量相关变量进行爬取并整理成一个CSV文件（AQI、质量等级、PM2.5、PM10、SO2、CO、NO2、O3_8h），数据来源：https://www.aqistudy.cn/historydata/index.php


## 背景
科研用途

## 数据描述
2013年12月~2018年6月（至今），383个城市的面板数据（383含缺失城市）

## 数据来源
https://www.aqistudy.cn/historydata/index.php

## 包含城市
阿坝州 阿克苏地区 阿拉善盟 阿勒泰地区 阿里地区 安康 安庆 安顺 安阳 鞍山 巴彦淖尔 巴中 白城 白沙 白山 白银 百色 蚌埠 包头 宝鸡 保定 保山 保亭 北海 北京 本溪 毕节 滨州 亳州 博州 沧州 昌都 昌吉州 昌江 常德 常熟 常州 朝阳 潮州 郴州 成都 承德 澄迈 池州 赤峰 崇左 滁州 楚雄州 达州 大理州 大连 大庆 大同 大兴安岭地区 丹东 儋州 德宏州 德阳 德州 迪庆州 定安 定西 东方 东莞 东营 鄂尔多斯 鄂州 恩施州 防城港 佛山 福州 抚顺 抚州 阜新 阜阳 富阳 甘南州 甘孜州 赣州 固原 广安 广元 广州 贵港 贵阳 桂林 果洛州 哈尔滨 哈密地区 海北州 海东地区 海口 海门 海南州 海西州 邯郸 汉中 杭州 合肥 和田地区 河池 河源 菏泽 贺州 鹤壁 鹤岗 黑河 衡水 衡阳 红河州 呼和浩特 呼伦贝尔 葫芦岛 湖州 怀化 淮安 淮北 淮南 黄冈 黄南州 黄山 黄石 惠州 鸡西 吉安 吉林 即墨 济南 济宁 佳木斯 嘉兴 嘉峪关 江门 江阴 胶南 胶州 焦作 揭阳 金昌 金华 金坛 锦州 晋城 晋中 荆门 荆州 景德镇 九江 酒泉 句容 喀什地区 开封 克拉玛依 克孜勒苏州 库尔勒 昆明 昆山 拉萨 来宾 莱芜 莱西 莱州 兰州 廊坊 乐东 乐山 丽江 丽水 溧阳 连云港 凉山州 辽阳 辽源 聊城 林芝 临安 临沧 临汾 临高 临夏州 临沂 陵水 柳州 六安 六盘水 龙岩 陇南 娄底 泸州 洛阳 漯河 吕梁 马鞍山 茂名 眉山 梅州 绵阳 牡丹江 那曲地区 南昌 南充 南京 南宁 南平 南通 南阳 内江 宁波 宁德 怒江州 攀枝花 盘锦 蓬莱 平顶山 平度 平凉 萍乡 莆田 濮阳 普洱 七台河 齐齐哈尔 黔东南州 黔南州 黔西南州 钦州 秦皇岛 青岛 清远 庆阳 琼海 琼中 衢州 曲靖 泉州 日喀则 日照 荣成 乳山 三门峡 三明 三亚 厦门 山南 汕头 汕尾 商洛 商丘 上海 上饶 韶关 邵阳 绍兴 深圳 沈阳 十堰 石河子 石家庄 石嘴山 寿光 双鸭山 朔州 四平 松原 苏州 绥化 随州 遂宁 塔城地区 台州 太仓 太原 泰安 泰州 唐山 天津 天水 铁岭 通化 通辽 铜川 铜陵 铜仁地区 吐鲁番地区 屯昌 瓦房店 万宁 威海 潍坊 渭南 温州 文昌 文登 文山州 乌海 乌兰察布 乌鲁木齐 无锡 芜湖 吴江 吴忠 梧州 五家渠 五指山 武汉 武威 西安 西宁 西双版纳州 锡林郭勒盟 咸宁 咸阳 湘潭 湘西州 襄阳 孝感 忻州 新乡 新余 信阳 邢台 兴安盟 宿迁 宿州 徐州 许昌 宣城 雅安 烟台 延安 延边州 盐城 扬州 阳江 阳泉 伊春 伊犁哈萨克州 宜宾 宜昌 宜春 宜兴 义乌 益阳 银川 鹰潭 营口 永州 榆林 玉林 玉树州 玉溪 岳阳 云浮 运城 枣庄 湛江 张家港 张家界 张家口 张掖 章丘 漳州 长春 长沙 长治 招远 昭通 肇庆 镇江 郑州 中山 中卫 重庆 舟山 周口 珠海 株洲 诸暨 驻马店 资阳 淄博 自贡 遵义 

## 数据输出
### 形如：
|index |aqi |city |co |no2 |o3 |pm10 |pm2_5 |quality |rank |so2 |time_point|
|----- |--- |---- |-- |--- |-- |---- |----- |------- |---- |--- |----------|
|0 |142 |北京 |2.6 |88 |11 |138 |109 |轻度污染 |53 |61 |2013-12-02|
|1 |86 |北京 |1.6 |54 |45 |86 |64 |良 |19 |38 |2013-12-03|
|2 |109 |北京 |2.0 |62 |23 |101 |82 |轻度污染 |29 |42 |2013-12-04|
|3 |56 |北京 |1.2 |38 |52 |56 |39 |良 |5 |30 |2013-12-05|
|…… |…… |…… |…… |……|……|…… |…… |…… |……|……|……|

## 缺失值
未知

## 笔者环境
python3.6.4  
xlrd  
pandas  
selenium  
chrome-68.0.3440.84  
chromedriver  



