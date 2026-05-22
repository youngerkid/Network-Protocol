# Network Protocol

本仓库用于学习网络协议底层原理，并按课程阶段保存笔记、实验记录和测试代码。

## 开发环境

| 工具 | 版本 |
| --- | --- |
| IDE | VSCode |
| JDK | JDK 21 |
| Tomcat | 11.0.22 |
| Maven | 3.9.16 |

## 目录结构

| 路径 | 用途 |
| --- | --- |
| `courses/` | 按五个阶段和 22 次课组织学习材料 |
| `docs/course-schedule.md` | 完整课表与阶段划分 |
| `docs/environment.md` | VSCode、JDK、Tomcat、Maven 环境说明 |
| `demo/` | Maven Web 测试集，用于验证 HTTP、Servlet 容器和部署实验 |

## 阶段划分

| 阶段 | 对应课次 | 重点 |
| --- | --- | --- |
| 第一阶段：网络基础 | 01-06 | 基本概念、网络设备、地址体系、路由、局域网、物理层与数据链路层 |
| 第二阶段：网络层与传输层 | 07-11 | UDP、TCP 可靠传输、流量控制、拥塞控制、连接建立与释放 |
| 第三阶段：应用层协议 | 12-16 | Socket、域名、DNS、DHCP、HTTP、请求头、响应头、状态码、Cookie、Session |
| 第四阶段：安全与加密 | 17-19 | 代理、CDN、网络安全、对称加密、非对称加密、数字签名、HTTPS |
| 第五阶段：现代网络协议扩展 | 20-22 | SPDY、QUIC、HTTP/2、HTTP/3、WebSocket、HTTPDNS、FTP、邮件、IPv6、流媒体、即时通讯、缓存 |

## 测试集构建

```powershell
cd demo
mvn clean package
```

构建产物为 `demo/target/demo.war`，可部署到 Tomcat 11.0.22。
