# DataAnalysis-SQLTableauPractice
## 分析欧美线上电商女鞋情况
### 项目背景和介绍
---
#### 背景：
kaggle/datafiniti 提供了一些欧美电商女鞋的产品信息数据，可以此来锻炼商业方面数据分析能力。主要用来实践 SQL、Tableau、PPT等。
#### 目的：
研究当时欧美电商售卖的女鞋特点、售出的女鞋特点，以及各品牌、网站的售卖情况。
#### 思路概要：
* 查看售卖、售出的女鞋的价格分布
* 分析女鞋的颜色、材质、尺寸分布情况
* 分析品牌售卖女鞋的情况
* 分析网站售卖女鞋的情况
#### 数据来源：
	[WomenShoes](https://www.kaggle.com/datafiniti/womens-shoes-prices)
	数据一共33801条，更新时间为 2016/01/01 - 2017/04/13。
			数据集包括鞋子名称，品牌，价格等。每个鞋子的每个价格都有一个条目，有些鞋子可能有多个条目。
				原表所有字段：id 	   asins	brand	categories	colors	count	dateAdded	dateUpdated	descriptions	dimension	ean	features	flavors	imageURLs	isbn	keys	manufacturer	manufacturerNumber	merchants	name	prices.amountMin	prices.amountMax	prices.availability	 prices.color	prices.condition	prices.count	prices.currency	 prices.dateAdded	prices.dateSeen	 prices.flavor	prices.isSale	prices.merchant 	prices.offer	prices.returnPolicy	 prices.shipping	prices.size	 prices.source	prices.sourceURLs	prices.warranty	 quantities	reviews	sizes	skus	sourceURLs	upc	vin	websiteIDs	weight		
#### 取其中需要的字段导入mySQL，各字段含义如下：
						id：				鞋编号
						brand：			品牌
						categories：		类别
						colors：			颜色
						dateAdded：		添加日期
						dateUpdated：	更新日期
						descriptions：	说明
						features：		特征
						keys: 			关键词
						manufacturer： 	供应商
						manufacturerNumber：供应商编号
						merchants：		销售商
						name：			鞋名称
						prices.amountMin：最低价格
						prices.amountMax：最高价格
						prices.condition：状态（新旧）
						prices.currency：货币
						prices.isSale：  是否销售
						prices.merchant ：销售渠道
						prices.size、sizes：鞋码（标准不同）

### 文件说明
---
	WSPRecord.txt 							数据分析记录（含SQL数据分析结果）
	OnlineWomenShoes.pptx 					项目展示
	--------------------------------------------------------
	WomenShoesPrices.txt 					kaggle数据说明
	womenshoe.csv 							所有女鞋数据
	SQL.txt 								SQL数据处理
	womenshoes.twbx，Tableaupractice.twb 	Tableau女鞋图表
