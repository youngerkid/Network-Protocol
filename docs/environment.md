# 开发环境

## 版本约定

| 工具 | 版本 |
| --- | --- |
| IDE | VSCode |
| JDK | JDK 21 |
| Tomcat | 11.0.22 |
| Maven | 3.9.16 |

## VSCode 建议

建议安装以下扩展：

- Extension Pack for Java
- Maven for Java
- XML
- Community Server Connectors

## Maven 测试集

`demo` 是本仓库的 Web 测试集，用于验证 HTTP、Tomcat 部署、请求响应和后续 Web 状态管理实验。

```powershell
cd demo
mvn clean package
```

生成的 WAR 文件位于：

```text
demo/target/demo.war
```

将该 WAR 部署到 Tomcat 11.0.22 后，访问对应上下文路径验证页面是否正常返回。
