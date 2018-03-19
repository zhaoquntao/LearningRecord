# LearningRecord
## 记录平时遇到的坑
## iOS相关
### 2018-3-19
#### double 转 NSString 的坑
#### 服务端给客户端返回数据一般使用 JSON 字符串 double 转为nsstring 后 出现的问题 例如:98.4 是98.40000000000001
解决办法如下:

```
double dpercent           = [dict[@"percent"] doubleValue];
NSString *precentL      = [NSString stringWithFormat:@"%.2f", dpercent];
NSDecimalNumber *num1 = [NSDecimalNumber decimalNumberWithString:precentL];
strD2   = [num1 stringValue];


```
## Swfit相关







## 前端相关
