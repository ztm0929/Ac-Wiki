# 网络空间安全————浏览网站安全

---
## https:// 与 http://

### 什么是 HTTPS？

- HTTPS 是一种在 Web 服务器和 Web 浏览器之间发送数据的安全方式。

超文本传输协议安全 (HTTPS) 是 HTTP 的安全版本，HTTP 是用于在 Web 浏览器和网站之间发送数据的主要协议。HTTPS 经过加密，以提高数据传输的安全性。当用户传输敏感数据（例如通过登录银行账户、电子邮件服务或健康保险提供商）时，这一点尤其重要。
任何网站都应使用 HTTPS，尤其是那些需要登录凭据的网站。在现代 Web 浏览器（例如 Chrome）中，未使用 HTTPS 的网站与使用 HTTPS 的网站的标记有所不同。URL 栏中如出现挂锁，则表示该网页是安全的。Web 浏览器非常重视 HTTPS；[Google Chrome 和其他浏览器将所有非 HTTPS 网站标记为不安全。](https://www.cloudflare.com/learning/ssl/why-use-https/)
![image](https://github.com/user-attachments/assets/7903824d-137b-4ceb-80d0-81325bbf5877)


### HTTPS 为什么很重要？如果网站没有 HTTPS，那会如何？

HTTPS 阻止网站以任何在网络上窥探的人都能轻松查看的方式广播信息。通过常规 HTTP 发送信息时，信息会分解为数据包，使用免费软件即可轻松“嗅探”这些数据包。这使得通过不安全的媒介（例如公共 Wi-Fi）进行的通信极易受到拦截。实际上，所有通过 HTTP 进行的通信都是以纯文本形式进行的，因而能够为任何使用正确工具的人轻松访问，而且容易遭受在途攻击。

使用 HTTPS 时，流量会经过加密，即使嗅探到数据包或以其他方式截取数据包，它们也会呈现为无意义的字符。我们来看一个例子：

> - 加密前：</br>

这是完全可读的文本字符串

> - 加密后：</br>

 ITM0IRyiEhVpa6VnKyExMiEgNveroyWBPlgGyfkflYjDaaFf/Kn3bo3OfghBPDWo6AfSHlNtL8N7ITEwIXc1gU5X73xMsJormzzXlwOyrCs+9XCPk63Y+z0= 

### HTTP 为什么不安全

- HTTP 由于是明文传输，主要存在三大风险

|     |         |
|:---:|:---:|
|1、 窃听风险 <br> 中间人可以获取到通信内容，由于内容是明文，所以获取明文后有安全风险 | ![image](https://github.com/user-attachments/assets/90d82d50-8d3c-4c7d-9f9b-e8b55ce89fb7) |
|2、 篡改风险 <br> 中间人可以篡改报文内容后再发送给对方，风险极大 |  ![image](https://github.com/user-attachments/assets/3ba95012-58be-4132-b9bd-31cda09bed3f) |
|3、 冒充风险 <br> 比如你以为是在和某宝通信，但实际上是在和一个钓鱼网站通信。 |   ![image](https://github.com/user-attachments/assets/1807e749-aa5d-4c5c-a21e-f1b342ef8a02) |

### 总结
增强安全性：HTTPS通过SSL/TLS协议对数据进行加密，保护用户数据不被窃取或篡改，确保通信的安全性。

提升信任度：使用HTTPS的网站更受用户信赖，因为它表明网站采取了额外的安全措施来保护用户隐私和数据。

浏览器支持：现代浏览器如Chrome将HTTP网站标记为“不安全”，而HTTPS网站则不会，这影响了用户对网站安全性的感知。

搜索引擎优化：搜索引擎倾向于提升使用HTTPS的网站的搜索排名，因为它们被认为是更安全、更可靠的资源。


## 常见域名（施工中）







## 参考文章

https://cloud.tencent.com/developer/article/1758154

https://www.cloudflare.com/zh-cn/learning/ssl/what-is-https/







 
