# 攻击次数

## 物理部分

此参数分为四个部分：
- 阵型
- 武将
- 武器类型
- 武器

次数范围
（`00-ff` 就是最大值为`255`）

攻击次数:

|属性|地址|值|
|--|--|--|
|阵型|806e0+阵型番号|次数|
|武器类型|806d0+武器类型番号|次数|
|武将|f8010+武将番号|次数|
|武器|f8110+武器番号|次数|

## 策略部分

此参数分为四个部分：
- 阵型
- 武将
- 武器类型
- 武器

次数范围
（`00-ff` 就是最大值为`255`）

攻击次数:

|属性|地址|值|
|--|--|--|
|阵型|806c0+阵型番号|次数|
|武器类型|806d8+武器类型番号|次数|
|武将|fb210+武将番号|次数|
|武器|fb310+武器番号|次数|

## 注意事项

- 武器类型·阵型必须有一个默认最小值为01 否则容易造成溢出bug 包括物理/策略
- 武器类型8个（00-07）00是无法装备任何武器 06扩展武器1 07扩展武器2
- 以上次数可叠加 叠加值就是攻击次数值