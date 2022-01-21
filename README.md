# 数据来源

　　数据来源于kaggle，链接：https://www.kaggle.com/c/GiveMeSomeCredit

# 数据探索

## 数据概况

### 训练集

|                                 type |    size | missing | unique |        |
| -----------------------------------: | ------: | ------: | -----: | ------ |
|                                   Id |   int64 |  150000 |  0.00% | 150000 |
|                     SeriousDlqin2yrs |   int64 |  150000 |  0.00% | 2      |
| RevolvingUtilizationOfUnsecuredLines | float64 |  150000 |  0.00% | 125728 |
|                                  age |   int64 |  150000 |  0.00% | 86     |
| NumberOfTime30-59DaysPastDueNotWorse |   int64 |  150000 |  0.00% | 16     |
|                            DebtRatio | float64 |  150000 |  0.00% | 114194 |
|                        MonthlyIncome | float64 |  150000 | 19.82% | 13594  |
|      NumberOfOpenCreditLinesAndLoans |   int64 |  150000 |  0.00% | 58     |
|              NumberOfTimes90DaysLate |   int64 |  150000 |  0.00% | 19     |
|         NumberRealEstateLoansOrLines |   int64 |  150000 |  0.00% | 28     |
| NumberOfTime60-89DaysPastDueNotWorse |   int64 |  150000 |  0.00% | 13     |
|                   NumberOfDependents | float64 |  150000 |  2.62% | 13     |

### 测试集

|                                 type |    size | missing |  unique |        |
| -----------------------------------: | ------: | ------: | ------: | ------ |
|                                   Id |   int64 |  101503 |   0.00% | 101503 |
|                     SeriousDlqin2yrs | float64 |  101503 | 100.00% | 0      |
| RevolvingUtilizationOfUnsecuredLines | float64 |  101503 |   0.00% | 85716  |
|                                  age |   int64 |  101503 |   0.00% | 82     |
| NumberOfTime30-59DaysPastDueNotWorse |   int64 |  101503 |   0.00% | 16     |
|                            DebtRatio | float64 |  101503 |   0.00% | 79878  |
|                        MonthlyIncome | float64 |  101503 |  19.81% | 11976  |
|      NumberOfOpenCreditLinesAndLoans |   int64 |  101503 |   0.00% | 56     |
|              NumberOfTimes90DaysLate |   int64 |  101503 |   0.00% | 18     |
|         NumberRealEstateLoansOrLines |   int64 |  101503 |   0.00% | 24     |
| NumberOfTime60-89DaysPastDueNotWorse |   int64 |  101503 |   0.00% | 12     |
|                   NumberOfDependents | float64 |  101503 |   2.59% | 13     |

## 描述性统计

### 训练集

|                                      |    count |         mean |          std |  min |          25% |          50% |           75% |       max |
| -----------------------------------: | -------: | -----------: | -----------: | ---: | -----------: | -----------: | ------------: | --------: |
|                                   Id | 150000.0 | 75000.500000 | 43301.414527 |  1.0 | 37500.750000 | 75000.500000 | 112500.250000 |  150000.0 |
|                     SeriousDlqin2yrs | 150000.0 |     0.066840 |     0.249746 |  0.0 |     0.000000 |     0.000000 |      0.000000 |       1.0 |
| RevolvingUtilizationOfUnsecuredLines | 150000.0 |     6.048438 |   249.755371 |  0.0 |     0.029867 |     0.154181 |      0.559046 |   50708.0 |
|                                  age | 150000.0 |    52.295207 |    14.771866 |  0.0 |    41.000000 |    52.000000 |     63.000000 |     109.0 |
| NumberOfTime30-59DaysPastDueNotWorse | 150000.0 |     0.421033 |     4.192781 |  0.0 |     0.000000 |     0.000000 |      0.000000 |      98.0 |
|                            DebtRatio | 150000.0 |   353.005076 |  2037.818523 |  0.0 |     0.175074 |     0.366508 |      0.868254 |  329664.0 |
|                        MonthlyIncome | 120269.0 |  6670.221237 | 14384.674215 |  0.0 |  3400.000000 |  5400.000000 |   8249.000000 | 3008750.0 |
|      NumberOfOpenCreditLinesAndLoans | 150000.0 |     8.452760 |     5.145951 |  0.0 |     5.000000 |     8.000000 |     11.000000 |      58.0 |
|              NumberOfTimes90DaysLate | 150000.0 |     0.265973 |     4.169304 |  0.0 |     0.000000 |     0.000000 |      0.000000 |      98.0 |
|         NumberRealEstateLoansOrLines | 150000.0 |     1.018240 |     1.129771 |  0.0 |     0.000000 |     1.000000 |      2.000000 |      54.0 |
| NumberOfTime60-89DaysPastDueNotWorse | 150000.0 |     0.240387 |     4.155179 |  0.0 |     0.000000 |     0.000000 |      0.000000 |      98.0 |
|                   NumberOfDependents | 146076.0 |     0.757222 |     1.115086 |  0.0 |     0.000000 |     0.000000 |      1.000000 |      20.0 |

### 测试集

|                                      |    count |         mean |          std |  min |          25% |          50% |          75% |       max |
| -----------------------------------: | -------: | -----------: | -----------: | ---: | -----------: | -----------: | -----------: | --------: |
|                                   Id | 101503.0 | 50752.000000 | 29301.536524 |  1.0 | 25376.500000 | 50752.000000 | 76127.500000 |  101503.0 |
|                     SeriousDlqin2yrs |      0.0 |          NaN |          NaN |  NaN |          NaN |          NaN |          NaN |       NaN |
| RevolvingUtilizationOfUnsecuredLines | 101503.0 |     5.310000 |   196.156039 |  0.0 |     0.030131 |     0.152586 |     0.564225 |   21821.0 |
|                                  age | 101503.0 |    52.405436 |    14.779756 | 21.0 |    41.000000 |    52.000000 |    63.000000 |     104.0 |
| NumberOfTime30-59DaysPastDueNotWorse | 101503.0 |     0.453770 |     4.538487 |  0.0 |     0.000000 |     0.000000 |     0.000000 |      98.0 |
|                            DebtRatio | 101503.0 |   344.475020 |  1632.595231 |  0.0 |     0.173423 |     0.364260 |     0.851619 |  268326.0 |
|                        MonthlyIncome |  81400.0 |  6855.035590 | 36508.600375 |  0.0 |  3408.000000 |  5400.000000 |  8200.000000 | 7727000.0 |
|      NumberOfOpenCreditLinesAndLoans | 101503.0 |     8.453514 |     5.144100 |  0.0 |     5.000000 |     8.000000 |    11.000000 |      85.0 |
|              NumberOfTimes90DaysLate | 101503.0 |     0.296691 |     4.515859 |  0.0 |     0.000000 |     0.000000 |     0.000000 |      98.0 |
|         NumberRealEstateLoansOrLines | 101503.0 |     1.013074 |     1.110253 |  0.0 |     0.000000 |     1.000000 |     2.000000 |      37.0 |
| NumberOfTime60-89DaysPastDueNotWorse | 101503.0 |     0.270317 |     4.503578 |  0.0 |     0.000000 |     0.000000 |     0.000000 |      98.0 |
|                   NumberOfDependents |  98877.0 |     0.769046 |     1.136778 |  0.0 |     0.000000 |     0.000000 |     1.000000 |      43.0 |







## 变量相关性

![heatmap](https://raw.githubusercontent.com/liangkaimeng/picture/main/heatmap.png)



# 特征工程

补充

# 模型搭建

补充

# 模型评估

补充

# 模型应用

补充

# 附录

补充

