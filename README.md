# 问题：[Kaggle信用卡反欺诈检测](https://www.kaggle.com/mlg-ulb/creditcardfraud)
> 项目简单描述：运用机器学习方法对信用卡的欺诈交易进行检测  
## 数据集  
> 数据集是典型的非均衡数据集，数据所含类别各自所占比例差异很大
## 两种思路  
> 1. 有监督学习在非均衡数据集上的运用（已经完成）  
> 2. futurework:无监督学习 —— 异常检测，学习中（待更新）  
## 两套工具  
> 1. 使用Scikit-learn和基于或兼容Scikit-learn的相关工具来实现  
> 2. 使用Pyspark和基于或兼容Pyspark的相关工具来实现
>>> A.Pyspark ML自带的Logistic Regression, LinearSVC, RandomForest, Naive Bayes, GBT等分类器自身带有一个参数weightCOL用于解决非均衡数据的问题;  
>>> B.Pyspark ML缺少与之对应的第三方特征选择工具，相比scikit-learn基于scikit-learn-contrib的强大生态，Pyspark ML的功能有些单薄;  
>>> C.正在寻找能够使scikit-learn并行运算的第三方库.  
## 代码快速浏览  
> [实现代码](https://nbviewer.jupyter.org/github/UTUnex/creditcard_anti_fraud_zh_CN/blob/master/%E6%9C%89%E7%9B%91%E7%9D%A3%E5%AD%A6%E4%B9%A0/with_feature_scaling_with_feature_selection.ipynb)  
## 注意  
> github有时候可能无法正常显示JupyterNotebook文件，此时请在浏览器中打开**https://nbviewer.jupyter.org/** ，然后将github中.ipynb文件的地址复制到搜索框中，然后点'go',进行浏览
