# Demo 测试集

`demo` 是本仓库的 Maven Web 测试集，用于配合网络协议课程做 HTTP、Tomcat 部署、请求响应、Cookie 和 Session 等实验。

## 环境

| 工具 | 版本 |
| --- | --- |
| JDK | 21 |
| Maven | 3.9.16 |
| Tomcat | 11.0.22 |

## 构建

```powershell
mvn clean package
```

构建成功后生成：

```text
target/demo.war
```
