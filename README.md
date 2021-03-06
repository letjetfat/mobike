#  摩拜上海城区用户使用数据

## 第一部分  总结

本可视化使用的是Tableau软件，使用的数据是2016年8月上海摩拜单车用户使用数据，其中主要展示了用户在工作日、周末的不同时段的单车使用数量和时长情况，发现在早、晚高峰及非高峰时段差异较大。

详情请查看[可视化文件](https://public.tableau.com/profile/.55935857#!/vizhome/mobike_V3/sheet0)



## 第二部分  设计

### 仪表板1：从整体月份来看单车使用情况在稳定增长

	仪表板1由每天单车使用总体情况(图1)和每天24小时单车使用情况(图2)构成。在图1中显示的是8月份整月的单车使用量，颜色由前浅逐渐变深，说明用户使用量在逐渐增多。在(图2)中显示的是汇总的24小时之内的单车使用情况条形图，每一个竖条都是该时段31天之内的记录汇总。可以看到在7-10点、17-20点，也就是早、晚高峰期阶段使用量大增。
	
	用鼠标选中(图1)的单元格后，可以在(图2)中看到当天24小时内的使用情况。在工作日，单车使用量仍然集中在早、晚高峰时段，说明共享单车已经在最后一公里出行上得到了人们的认可。在周末，使用量差异没有工作日大，但峰值仍在出现在17-20点之间。

### 仪表板2：从每天的数据来看使用量和使用时长都在增长

	仪表2由每天单车使用数量(图1)和每天单车使用总量、单车使用总时间、每次使用时间均值(图2)组成。图1显示的是整个月份逐天使用量情况，明显看到使用量的稳定增长趋势。图2是总使用时长条形图和平均使用时长折线图构成，从条形图上可以看到总使用时长也在稳定增长，平均每天每次单车使用时长在16分钟左右波动，差异较小，说明了单车使用主要是短距离出行。

### 仪表板3：从整个月份来看单车使用时长

仪表板3由每天单车使用总时长(图1)和3个小条形图构成。3个小条形图展示的是在24小时之内使用总时长、使用量、平均使用时长的情况。通过选中图1中的天数可以在下方3个小图中展示当天的情况，可以看到使用在7-10、17-20时间段，单车使用情况都比相邻时间段多很多。但在平均使用时长上，却是7-10点上班时段最短，平均使用时长只有10分钟左右，这表明了用户已经在最后一公里出行上充分利用好了共享单车。

### 仪表板4：每天单车使用时长分布

仪表板4由不同时段内单车平均使用时长(图1)，单车骑士时长分布(图2)组成。同意通过筛选天数和时间段来查看单车骑行时长的分布，整体上来看骑行时长在10、20、30分钟内的短距离出行占据了80%以上，在10分钟以内的出行占比接近50%。

### 仪表板5：工作日、周末骑行次数和时长情况

	仪表板5由工作日、周末不同时间段骑行单车情况小多组图构成。横坐标是骑行的次数，纵坐标是每次骑行的平均时长。
	
	就工作日来说，用户在早高峰和晚高峰期内平均单车数量都为2次左右，早高峰使用时间都比较短，而晚高峰使用时长较长，非高峰期使用平均数量为3次，但时长相比晚高峰时要短。
	
	就不同时段的周末和工作日使用情况看，在同一非高峰期、早高峰、晚高峰时段，平均骑行时长都是周末稍长，但周末的平均使用次数却比工作日要少一些，而且整体使用数量上，周末的使用次数也集中偏小，反映了除了用户在工作日使用次数多而使用时间短，在周末使用次数少而使用时间长的规律。而且就单个小多组图来看，也呈现出使用次数越多的用户使用时长越短的趋势。

### 仪表板6：查看用户骑行的单车的轨迹

仪表6可以通过筛选不同的用户，以及不同的骑行时间长度来查看用户骑行的轨迹



###### 说明:

摩拜单车上海用户数据[原始数据](https://pan.baidu.com/s/1MLOx9xFEh1Hge3S5XdtqvA)， 使用Python清理后并将骑行轨迹数据提取后，将宽型数据转换成长型数据文件[长格式数据](https://pan.baidu.com/s/11S_yxZ5ifjG-JSRtQ6xZqA)，本次用Tableau可视化时使用的是经过转换后的[长格式数据](https://pan.baidu.com/s/11S_yxZ5ifjG-JSRtQ6xZqA)，当然如果不想分析用户的骑行轨迹的也可以使用[原始数据](https://pan.baidu.com/s/1MLOx9xFEh1Hge3S5XdtqvA)，需要数据的可以点击链接到百度网盘里下载。