### 股票盈亏监视器 - 命令行版
- 根据持仓数量和成本价格实时展示当前盈亏和百分比
- 支持动态修改配置文件，不用重启程序
- 根据需要调整结果展示频率
- Python2.7测试通过
```

#### 依赖
- 第三方网络库requests

#### JSON 配置文件  
```
code: 股票代码  
name: 股票名称，最终显示到结果中  
share: 现在持有数量  
cost: 现在持有的每股成本  
例如：
[
  {
    "code":"sz002432",
    "name":"九安医疗",
    "share": 200,
    "cost": 7.575
  },
  {
    "code":"sh600846",
    "name":"同济科技",
    "share": 200,
    "cost": 8.465
  }

]
```

#### 运行结果
- python main.py
- 刷新频率默认为60秒
- 结果如下
```
九安医疗  |  sz002432  |  15.0  |  0.99 %
---------------------------------------------
同济科技  |  sh600846  |  49.0  |  2.89 %
```
    
    

