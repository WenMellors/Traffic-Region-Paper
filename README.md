<style>
	table th:first-of-type {
		width: 60px;
	}
    table th:nth-of-type(2) {
    	width: 60px;    
    }
    table th:nth-of-type(3) {
    	width: 60px;    
    }
    table th:nth-of-type(3) {
        width: 100px;
    }
</style>

## WWW

#### 论文简介

| 编号        | 名称     | 年份 | 源码链接                                    | 简介                                                         |
| ----------- | -------- | ---- | ------------------------------------------- | ------------------------------------------------------------ |
| [1](#WWW-1) | FPMC     | 2010 | [非官方](https://github.com/khesui/FPMC)    | 实际是推荐系统相关的方法，但也可以用来做下一跳预测。基于马尔科夫链+矩阵分解来实现的 |
| [2](#WWW-1) | DeepMove | 2018 | [链接](https://github.com/vonfeng/DeepMove) | 引入历史轨迹特征，并用 attention 机制去处理它                |

#### 论文编号

1. **<span id = "WWW-1">Factorizing Personalized Markov Chains for Next-Basket Recommendation</span>**
2. **<span id="WWW-2">DeepMove: Predicting Human Mobility with Attentional Recurrent Networks</span>**

## KDD

#### 论文简介

| 编号           | 名称 | 年份 | 源码链接 | 简介                               |
| -------------- | ---------- | ----------------------------------------- | ----------------------------------------- | ----------------------------------------- |
| [1](#KDD-1) | MTGNN | 2020 | [链接](https://github.com/nnzhan/MTGNN) | 使用 GCN + 1dCNN 来实现，可以进行多步预测 |
| [2](#KDD-2)   | GeoSAN | 2020 | [链接](https://github.com/libertyeagle/GeoSAN) | 使用图来做 encoder，以及一种新的 loss function 来做下一跳推荐 |


#### 论文编号

1. **<span id="KDD-1">Connecting the Dots: Multivariate Time Series Forecasting with Graph Neural Networks</span>**
2. **<span id = "KDD-2">Geography-Aware Sequential Location Recommendation</span>**

## ICDM

#### 论文简介

| 编号         | 名称 | 年份 | 源码链接                               | 简介                                                         |
| ------------ | ---- | ---- | -------------------------------------- | ------------------------------------------------------------ |
| [1](#ICDM-1) | TMCA | 2018 | [链接](https://github.com/zhenql/TMCA) | 相关，是做下一跳 POI 预测的。使用 LSTM 来做 encoder-decoder，以及引入 attention 机制 |

#### 论文编号

1. **<span id = "ICDM-1">Next Point-of-Interest Recommendation with Temporal and Multi-level Context Attention</span>**

## CIKM（B 类会议）

#### 论文简介

| 编号         | 名称 | 年份 | 源码链接                                 | 简介                                            |
| ------------ | ---- | ---- | ---------------------------------------- | ----------------------------------------------- |
| [1](#CIKM-1) | SERM | 2017 | [链接](https://github.com/yaodi833/serm) | 引入额外的 POI 信息或其他文本数据进行下一跳预测 |

#### 论文编号

1. **<span id = "CIKM-1">SERM: A Recurrent Model for Next Location Prediction in Semantic Trajectories</span>**