## gas 变化的记录
**Before**

|      | Transaction gas | Execution gas |
| ---- | --------------- | ------------- |
|1 | 23037 |  1765 |
|2 | 23825 |  2553 | 
|3 | 24613 |  3341 |
|4 | 25401 |  4129 |
|5 | 26189 |  4917 |
|6 | 26977 |  5705 |
|7 | 27765 |  6493 |
|8 | 28553 |  7281 |
|9 | 29341 |  8069 |
|10 | 30129 |  8857 |


**after **

|      | Transaction gas | Execution gas |
| ---- | --------------- | ------------- |
|1 | 22210 |  938 |
|2 | 22210 |  938 | 
|3 | 22210 |  938 |
|4 | 22210 |  938 |
|5 | 22210 |  938 |
|6 | 22210 |  938 |
|7 | 22210 |  938 |
|8 | 22210 |  938 |
|9 | 22210 |  938 |
|10 | 22210 | 938 |

## calculateRunway() 函数的优化思路

将 totalSalary 当做合约属性, 每次增删改查 employee 的时候更新,这样就不必每次执行 caculateRunway 的时候都遍历计算一遍,确保 totalSalary 计算最小的次数