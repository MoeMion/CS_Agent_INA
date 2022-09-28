# CS_Agent_INA
CS 4.5 Java Agent INA  理论支持CS4.X版本

## 更新记录:

cs_agent_0.0.2   

```
0、各功能理论完全分离、可单独进行开启关闭。
1、支持CS4.5 crack_auth  【配置need.crack_auth 可选 Y/N】
2、支持CS4.5 原版汉化  【配置need.translation 可选 Y/N】
3、支持CS4.5 XSS RCE修复  【配置need.fix_xss_rce 可选 Y/N】
4、支持CS4.5 javaagent调试限制绕过  【配置need.crack_agent 可选 Y/N】
5、支持自定义配置文件名称  【可选 -javaagent:cs_agent.jar=config.ini 】
```

cs_agent_0.0.4

```
1、修复代码逻辑, 当不开启翻译功能时，可删除resources和scripts目录
```

cs_agent_0.0.5

```
1、当配置文件不存在时，支持生成默认配置文件。 且配置文件不存在时，会进行跳过，即本次不进行agent劫持

2、实现所有参数通过配置文件指定。 注意：不再可以指定jar包的内的路径，且初始化时为了不影响启动，会清除实际使用的文件，再进行拷贝。
```



## 使用方法：

```
0、根据需求配置config.ini
1、使用默认配置文件config.ini 【-javaagent:cs_agent.jar】
2、使用自定义配置文件名称custom.ini 【-javaagent:cs_agent.jar=custom.ini】
```

## 声明

```
1、非完全原创代码, 整合于CSAgent、Attack2DefenseAgent、CVE-2022-39197 patch
2、本工具仅供学习研究、如您在使用本工具的过程中存在任何非法行为，您需自行承担相应后果，我们将不承担任何法律及连带责任。
3、临时开放项目,如程序稳定运行,未出现BUG，将在一段时间后删除。
```

