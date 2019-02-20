---
title: Echarts Map地图
date: 2018-03-29 17:16:59
tags: echarts,map
categories: Echarts
copyright: true
---

# Echarts Map地图

>1. [简介（心得总结）](#简介（心得总结）)
1. [效果展示](#效果展示)
    1. [业务代码实现](#业务代码实现)


## 简介（心得总结）
 虽然echarts在同类型的数据可视化框架中还算是比较的简单易用的，但是在入手的时候可能也会有一些比较麻烦的地方困扰着你，比如文档这么多我怎么看，实例已经比较齐全了我还需要看API文档吗，这些问题我想在这里统一的说一下，其实echarts的学习无外乎就是先了解一下框架大致上的分类，然后是在将全部的API阅读一遍，使对框架有一个全局的认识，然后在通过实践去深入学习，示例只不过是这一步的一个辅助而已，只有扎扎实实的通过学习API一步一个脚印去了解学习，才能做到在使用的时候心中有底。

 Echarts 地图参考官方文档：[Map地图](http://echarts.baidu.com/examples/#chart-type-map)

## 效果展示

#### 在线预览：[点击此处可在线预览效果](http://218.4.136.114:7009/H5/Attaches/Echarts图表/地图/示例源码/echarts/echarts_map.html)

![](http://218.4.136.114:7009/H5/epointmobileWiKi/assets/005/20180329-f11bd03c.png)  

## 业务代码实现

#### 一、[点击此处进行示例demo源码下载](http://218.4.136.114:7009/H5/Attaches/Echarts图表/地图/示例源码/echarts.zip)

#### 二、在线阅读源码
#####  `(友情提醒：以下代码请根据实际项目自行参考，勿直接复制运行)`
##### 1. 引入第三方图表库echarts.js
```javascript
<script type="text/javascript" src="你自己的/js/echarts.js" ></script>
```
##### 2. 具体代码

```javascript
/**
 * 作者： 孙尊路
 * 创建时间： 2018-03-29 10:54:19
 * 版本： [1.0, 2018/3/29]
 * 描述： Echarts 地图
 */

'use strict';
Util.loadJs([], function() {
	//初始化数据
	customBiz.initData();
});

var customBiz = {
	/**
	 * @description 初始化数据
	 */
	initData: function() {
		var self = this;
		var myChart = echarts.init(document.getElementById('main'));
		myChart.showLoading();
		var mapFeatures = echarts.registerMap('suzhou', "参考官方Echarts Map配置");
		myChart.hideLoading();
		myChart.setOption(self.configOption());
	},
	configOption: function() {
		// 声明常用配置项
		var name_title = ""
		var subname = '';
		var nameColor = " rgb(55, 75, 113)";
		var name_fontFamily = '宋体';
		var name_fontSize = 20;
		var mapName = 'china';
		var data = [];
		var toolTipData = [{
				name: '常熟市',
				value: [{
					"name": "家庭走访率",
					"value": 90
				}, {
					"name": "已走访居民家庭",
					"value": 63
				}, {
					"name": "收集问题",
					"value": 15
				}, {
					"name": "已解决问题",
					"value": 13
				}]
			},
			{
				name: '虎丘区',
				value: [{
					"name": "家庭走访率",
					"value": 13
				}, {
					"name": "已走访居民家庭",
					"value": 63
				}, {
					"name": "收集问题",
					"value": 15
				}, {
					"name": "已解决问题",
					"value": 13
				}]
			},
			{
				name: '昆山市',
				value: [{
					"name": "家庭走访率",
					"value": 13
				}, {
					"name": "已走访居民家庭",
					"value": 63
				}, {
					"name": "收集问题",
					"value": 15
				}, {
					"name": "已解决问题",
					"value": 13
				}]
			},
			{
				name: '太仓市',
				value: [{
					"name": "家庭走访率",
					"value": 90
				}, {
					"name": "已走访居民家庭",
					"value": 63
				}, {
					"name": "收集问题",
					"value": 15
				}, {
					"name": "已解决问题",
					"value": 13
				}]
			},
			{
				name: '吴江区',
				value: [{
					"name": "家庭走访率",
					"value": 90
				}, {
					"name": "已走访居民家庭",
					"value": 63
				}, {
					"name": "收集问题",
					"value": 15
				}, {
					"name": "已解决问题",
					"value": 13
				}]
			},
			{
				name: '相城区',
				value: [{
					"name": "家庭走访率",
					"value": 13
				}, {
					"name": "已走访居民家庭",
					"value": 63
				}, {
					"name": "收集问题",
					"value": 15
				}, {
					"name": "已解决问题",
					"value": 13
				}]
			},
			{
				name: '张家港市',
				value: [{
					"name": "家庭走访率",
					"value": 13
				}, {
					"name": "已走访居民家庭",
					"value": 63
				}, {
					"name": "收集问题",
					"value": 15
				}, {
					"name": "已解决问题",
					"value": 13
				}]
			},
			{
				name: '吴中区',
				value: [{
					"name": "家庭走访率",
					"value": 13
				}, {
					"name": "已走访居民家庭",
					"value": 63
				}, {
					"name": "收集问题",
					"value": 15
				}, {
					"name": "已解决问题",
					"value": 13
				}]
			},
			{
				name: '姑苏区',
				value: [{
					"name": "家庭走访率",
					"value": 13
				}, {
					"name": "已走访居民家庭",
					"value": 63
				}, {
					"name": "收集问题",
					"value": 15
				}, {
					"name": "已解决问题",
					"value": 13
				}]
			}
		];

		// 配置项
		var options = {
			title: {
				text: name_title,
				subtext: subname,
				x: 'center',
				textStyle: {
					color: nameColor,
					fontFamily: name_fontFamily,
					fontSize: name_fontSize
				}
			},
			tooltip: {
				// 提示框
				trigger: 'item',
				formatter: function(params) {
					var toolTiphtml = ''
					for(var i = 0; i < toolTipData.length; i++) {
						// 张家港市=张家港市的数据
						if(params.name == toolTipData[i].name) {
							toolTiphtml += toolTipData[i].name + ':<br>'
							for(var j = 0; j < toolTipData[i].value.length; j++) {
								if(j == 0) {
									toolTiphtml += toolTipData[i].value[j].name + ':' + toolTipData[i].value[j].value + "%<br>"
								} else {
									toolTiphtml += toolTipData[i].value[j].name + ':' + toolTipData[i].value[j].value + "万<br>"

								}
							}
						}
					}
					return toolTiphtml;

				}
			},
			/**
			 * 描述：图例组件展现了不同系列的标记(symbol)，颜色和名字。可以通过点击图例控制哪些系列不显示。
			 */
			legend: {
				orient: 'vertical',
				y: 'bottom',
				x: 'right',
				textStyle: {
					color: '#fff'
				}
			},
			/**
			 * 描述：visualMap 是视觉映射组件，用于进行『视觉编码』，也就是将数据映射到视觉元素（视觉通道）。
			 * 链接：http://echarts.baidu.com/option.html#visualMap
			 */
			visualMap: {
				type: 'continuous',
				min: 0,
				max: 10000,
				text: ['High', 'Low'],
				realtime: true,
				calculable: true,
				color: ['orangered', 'yellow', 'lightskyblue']
			},
			/*工具按钮组*/
			toolbox: {
				/** 暂时注释
				show: true,
				orient: 'vertical',
				left: 'right',
				top: 'center',
				feature: {
					dataView: {
						readOnly: false
					},
					restore: {},
					saveAsImage: {}
				}
				**/
			},
			series: [{
				type: 'map',
				mapType: "suzhou",
				label: {
					normal: {
						show: true
					},
					emphasis: {
						textStyle: {
							color: '#000',
							fontSize: 12
						}
					}
				},
				itemStyle: {
					normal: {
						borderColor: '#58b7ab',
						areaColor: '#fff',
					},
					emphasis: {
						areaColor: '#ffd200',
						borderWidth: 0
					}
				},
				animation: false,
				data: [{
						name: '常熟市',
						value: 100
					},
					{
						name: '虎丘区',
						value: 500
					},
					{
						name: '昆山市',
						value: 300
					},
					{
						name: '太仓市',
						value: 400
					},
					{
						name: '吴江区',
						value: 500
					},
					{
						name: '相城区',
						value: 600
					},
					{
						name: '张家港市',
						value: 700
					},
					{
						name: '吴中区',
						value: 800
					},
					{
						name: '姑苏区',
						value: 900
					}
				]
			}],

		}

		return options;
	}

}
```
