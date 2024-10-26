# 网络空间安全—密码管理Part1
## part1更新状态：✅
## part2：❌
## part3：❌
* 随着网络空间安全危害事件的发生，密码作为个人信息账号的第一道防线，应该得到重视。
* 很多人都有这个经历：
 > * https://linux.do/t/topic/235317
 > * https://linux.do/t/topic/239657
 > * https://linux.do/t/topic/235505
* 如果你频繁使用一个账户密码，且缺少二次验证，攻击者可以使用撞库等手段，破解你几乎所有的账号。
* 下面，以Android为主，MacOS为辅，通过各种手段，加强账号信息强度：

## 检查密码强度：
> 1. 你是不是经常在各大网站使用同一个密码？
> 2. 你的密码是不是和个人姓名，生日等等息息相关？
> 3. 你的密码是不是只存储在浏览器里？
### 开源密码强度检测软件：
![](https://f-droid.org/repo/com.cyb3rko.pazzword/en-US/icon_4TlGVCx28WCvT9UWJJd3LIJnGxbG0XnQgrMEhJKROYc=.png)
**Pazzword**
[**Github**](https://github.com/cyb3rko/pazzword)
[**F-Droid**](https://f-droid.org/zh_Hant/packages/com.cyb3rko.pazzword/index.html)
[**G-Play**](https://play.google.com/store/apps/details?id=com.cyb3rko.pazzword&hl=zh)
输入你常用的(不放心可以输修改后的)密码，
### **可以得到诸如**：
> 1.  密码是否安全
> 2. 密码是否常见
> 3. 加密指数
> 4. 修改建议
> 5. 是否含有字典关键词
> 6. 破解猜测次数,时长

比如密码：**neoisgreat**
  > * Guesses：1.69X10^8
  > * Offline MD5 ：瞬间
  > * Offline SHA512 ：瞬间
  > * Offline bcrypt10：7min
  > * Offline bcrypt14：1h
  > * Online Unthrottled：3days
  > * Online Throttled：2 years
同时配备强密码生成器，但不推荐，因为有更好的方法，生成管理强密码；

### 强大的开源密码管理器：
![](https://www.keepassdx.com/assets/img/keepassdx.svg)
## KeePassDX
[**F-Droid**](https://f-droid.org/packages/com.kunzisoft.keepass.libre/)
[**G-Play**](https://play.google.com/store/apps/details?id=com.kunzisoft.keepass.free)
[**Github**](https://github.com/Kunzisoft/KeePassDX/releases)
### 优点：
* 安全性高
  * 数据不存储在云端，而是在本地仓库![OD8znB.png](https://ooo.0x0.ooo/2024/10/26/OD8znB.png)
  * 自主选择加密方式，任意搭配开启关闭**密码登陆，指纹解锁，密钥文件，实物密钥**
 (密钥文件可在termux生成)
 ![OD8F4s.png](https://ooo.0x0.ooo/2024/10/26/OD8F4s.png)
* 定制化程度高
  * 作为赛博人，软件安全性固然重要，但我们也不想使用一款难看的老式UI软件，KeePassDX提供内置图标和自定义图标，让密码管理也能乐在其中。
![OD87YN.png](https://ooo.0x0.ooo/2024/10/26/OD87YN.png)
* 迁移能力强
  * 由于密码都存储在一个文件里(当然你也可以搭建更多个数据库存储不同密码)，我们迁移密码只需要将密码数据库和密钥文件移动到目的地，搭配不同平台不同软件都可以直接使用(图标包会存储在.kdbx文件)
  * 比如我在Android端，将文件，密钥迁移到MacOS，只需要下载MacPass或者KeePassXC等开源软件，导入数据即可使用。
  * 使用resillion sync或syncthing可以高效的同步密码库，多端同步
### 缺点：
* ALL IN BOOM
  * 正因为密码存储在数据库文件，如果误删密码库，要么去找文件恢复软件，要么从其他地方备份，要么......寄！
  * 所以，要开启不同的登陆验证方式，勤备份文件到安全的地方，多端同步。

<details>
<summary>关于作者</summary>

> 文章地址：  

Linuxdo

https://linux.do/t/topic/242686

Acwiki

https://github.com/KipJayChou/AcWiKi/blob/main/03-tools/cyber%20security/password_manage1.md

> 作者：  

user695(linux.do)  

https://linux.do/u/user695/summary  

KipJaychou(Github)

https://github.com/KipJayChou

> 向我申请Linuxdo邀请码：  

jay20070220@gmail.com

</details>
