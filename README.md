<h1 align="center">一本 HTTP 的漫画：《图解 HTTP》</h1>
yangyangwithgnu@yeah.net  
http://yangyangwithgnu.github.io/  
2016-09-05 22:52:32


##谢谢

**捐赠：支付宝 yangyangwithgnu@yeah.net ，支付宝二维码（左），微信二维码（右）**
<div align="center">
<img src="https://raw.githubusercontent.com/yangyangwithgnu/yangyangwithgnu.github.io/master/pics/alipay_donate_qr.png" alt=""/>
<img src="https://raw.githubusercontent.com/yangyangwithgnu/yangyangwithgnu.github.io/master/pics/wechat_donate_qr.png" alt=""/><br>
</div>

**二手书**：书，我提高开发技能的重要手段之一，随着职业生涯的发展，书籍也在不断增多，对我而言，一本书最多读三遍，再往后，几乎没有什么营养吸收，这部分书对我已基本无用，但对其他人可能仍有价值，所以，为合理利用资源，我决定低价出售这些书，希望达到两个目的：0）用售出的钱购买更多新书（没当过雷锋的朋友 (๑´ڡ`๑)）；1）你低价购得需要的书（虽然二手）。到 https://github.com/yangyangwithgnu/used_books 看看有无你钟意的。


##公告

**讨论**：任何意见建议 yangyangwithgnu@yeah.net  



一本 HTTP 的漫画：《图解 HTTP》

web 安全是个涉及面非常广的领域，web 架构及其组件、HTTP 协议、前后端 web 开发语言、OWASP top10 漏洞、各类安全工具、脚本语言等等全是 web 安全的基础要求，如果你都不熟悉，最先学习的我建议是 HTTP 协议。一方面，它是整个 web 的基石，是其他基础知识的基础，另一方面，它本身是比较简单的协议，并无多少难度，只要辅以好的书籍和工具，可以较快的熟悉 HTTP。

HTTP 协议可能是你最熟悉（每次访问网站前你都会输入 http://）的陌生人（常用的 HTTP 方法有哪些？），虽然接触得多，但不见得了解。目前市面上讲解 HTTP 的名著当属 David Gourley 等人合著的《HTTP: The Definitive Guide》（中译《HTTP权威指南》），是一本快 700 页的大部头书。我本人倒没“大部头书籍畏惧症”，不过，在系统学习一个陌生领域前，我的习惯是，先找一本入门级书籍进行知识铺垫，好的入门书应该具备如下几个特点：尽可能多的专业术语，最好能中英文对照，先对术语混个眼熟；对术语有浅显易懂的解释，甚至融入上下文之中，用实例讲解概念；有丰富的插图，用画面加深记忆；话语平实，少用说教的语气。《图解 HTTP》是这样一本讲解 HTTP 协议的不错入门书籍：
（《图解 HTTP》封面）

总的说来，《图解 HTTP》是本让人很轻松就能读完的小书，主要受众是那些完全没接触 HTTP 报文，不明白浏览器与网站之间如何通信的读者。聚焦到 web 安全领域，如果你对代理拦劫工具（如，ZAP、Burp Suite）捕获到的 HTTP 报文头感到完全陌生的，那么这本《图解 HTTP》非常适合你，完全不需要任何背景知识。该书行文轻松，完全消除你学习协议的恐惧感，全书大量插图，加之作者是日本人，你会发现，其实在看一本漫画书，或许这就是这本小书的最大优点。当然，缺点也很明显，知识点将得不够深入透彻，缺少可动手实操的例子，我觉得，作者在讲解 HTTP 状态码（第四章）、HTTP 头（第六章）、认证（第八章）时应该配以 HTTP 抓包工具（如，ZAP）分析报文的操作步骤，把网络上的 HTTP 报文实实在在的放在读者眼前，消除陌生感。

《图解 HTTP》原著作者是上野宣先生，中译者是于均良。上野宣先生，OWASP 日本区负责人，长期从事安全相关咨询和培训工作，在日本 web 安全领域拥有很高人气，他以安全人员视角写的 HTTP 书，正是我需要的；于均良，网上资料不多，上海交大的硕士，高级软件工程师。

对于计算机书籍，我倾向尽可能看原版，前提是，英文原版。《图解 HTTP》原版是日文，我就只能“屈尊”看看中译吧。刚看那会儿，我只希望别把关键概念翻译错就行了，现在看完后，我想大声告诉你，于均良翻译的书，绝对品质保障。我的天，这是我看到的第一本全无翻译的痕迹的译作，甚至超过侯捷先生。

全书共十一章，以 HTTP 与 web 的关系开篇，以 web 安全结题。

第一章，了解 web 及网络基础。由于开发门槛低、运维成本低，web 如今已成为互联网的主要内容源。web 系统有三个要素：HTML、URL、HTTP。HTML，超文本标签语言，web 内容的具体呈现的形式；
URL，统一资源定位符，用于寻址 HTML 的路径；HTTP，超文本传输协议，将 HTML 从位于 URL 的服务端传输至客户端的载体。本章主要介绍了 web 的三要素、HTTP 历史、以及其他相关协议。

第二章，简单的 HTTP 协议。以客户端请求、服务端应答的全流程，演示了 HTTP 报文的生命周期。

第三章，HTTP 报文内的 HTTP 信息。本章讲述了一个 HTTP 完整报文的格式。

第四章，返回结果的 HTTP 状态码。服务端的每次应答均有标识其结果的代号，即状态码，比如，2xx 代表成功相关、3xx 代表重定向相关、4xx 代表客户端请求错误相关、5xx 代表服务端内部错误相关。

第五章，与 HTTP 协作的 web 服务器。本章简要介绍了与 web 应用服务器配套的代理、网关、隧道、缓存等机制及其程序。

第六章，HTTP 首部。这个术语不太习惯，我更喜欢称为 HTTP 头 ：）。HTTP 报文分为 HTTP 头和 HTTP 体两部分，可以说 HTTP 头是整个报文的核心。本章介绍了 HTTP 头中常见的字段，阅读时可以逐一过一遍，记不住没关系，后续需要时再当作手册进行查阅。

第七章，确保 web 安全的 HTTPS。HTTP 是明文传输协议，当然你也可以在业务逻辑中实现加密传输，但这毕竟不是协议自身支持的。通过将 HTTP 放入 SSL 中，后来实现了 HTTPS。HTTPS 主要两个目的，一是证明谁是谁、二是传输报文加密。

第八章，HTTP 是种无状态协议，涉及需要体现状态的场景（如，登录状态），通过做法是在客户端保存 cookie、服务端保存 session（会话），以体现用户的各类状态信息。早前使用的基础认证（basic authentication）和摘要认证（digest authentication）现在已经很少使用了，目前基本上采用基于表单的认证机制（form-based authentication）,另外，还有 windows 的 NTLM 认证、keberos 认证。

第九章，基于 HTTP 的功能追加协议。HTTP 是 20 多年前的产物，当前的使用场景难免与开发初衷有些出入，比如，页面中部分信息更新了，不得不重新获取整个页面，导致传输无用数据，随之产生的 AJAX 技术有效解决了这类问题；又比如，HTTP 是客户端发起请求，服务端返回应答，完全的单向联系，若要及时了解服务端是否有更新，只能在客户端轮询请求，效率肯定低下，websocket 应运而生，实现 HTTP 基础上的全双工通信；再如，随着 web 系统在企业用户中的普及，在线文档编辑成了常见需求，webDAV 实现了多人共享在线文档编辑的能力。

第十章，构建 web 内容的技术。web 内容的主体是 HTML，操纵 HTML 需要 javascript、DOM、CSS 等前段技术，生成 HTML 就需要 PHP、JSP、ASP 等后端语言；另外，web 常用的 XML、RSS/atom、JSON 等数据交互技术也作了简介。

第十一章，web 的攻击技术。这是全书最吸引我的章节，毕竟，深入掌握 web 安全是让我学习 HTTP 的主要驱动力。本章主要介绍了如下主题：
* web 系统成为安全问题频发重灾区的原因。大概三方面：一是，HTTP 是个年代久远的协议，设计初衷只是为了文本信息的传输，并不含有加密、认证等等安全机制，现有 web 系统的认证均是在规范之外自行实现的，难免千疮百孔；二是，HTTP 作为 web 的载体，整个传输过程，对于任何人都是可见的、甚至是可篡改的，换言之，服务端接收到客户端的任何输入均是不可信的，这让安全机制防御面无形中增大了许多；三是，web 系统本身开发门槛很低，任何技术背景的人都可以在短时间内开发出一个所谓的业务系统网站，web 系统的数量俱增，稍为有点安全基础的人员，可以找到大量存在高危隐患的 web 系统；
* 几种常见的注入攻击。前面提过，任何输入皆不可信，这直接导致出现注入攻击。所谓注入，就是在系统生成的原始信息中，加入特意构造的恶意信息，以达到扰乱服务端正常处理逻辑的目的。所以，对任何输入，服务端都应进行安全校验。很多人会纠结是否任何校验逻辑都应放在服务端？本书给出了很好的答案：输入有效性校验，应在客户端和服务端都执行，客户端执行为了提升用户体验（比如，该填手机号的字段填入了非数字，如果没有客户端校验，那么要等到服务端校验后再返回，耗时太长，而且如果该页面有其他多个字段，又得全部重填），服务端执行是为了增强安全性。同时，作者还对 XSS、iSQL、OS 命令注入、HTTP 头注入、邮件头注入、目录遍历、远程文件包含等常见注入型漏洞辅以案例讲解，虽然都是点到为止，但，让从未接触过这些概念的读者有了比较直观的了解。
* 几种常见的设计缺陷。一是，文件名可猜测，比如，以日期命名的日志文件，http://my.website.com/20160904.log ，很容易猜测到任意日期的日志文件；二是，系统输出了有价值的报错信息，比如，登录某网站时，你输入的账号和密码有误，网站提示说账号不存在，这就让攻击者基于此猜测出大量有效账号，大大提供后续密码攻击的成功率；三是，开放重定向，某些网站允许重定向至站外连接，这让攻击者可以将恶意网站地址混入正规网站 URL 之中，达到欺骗用户的目的。
* 几种常见的会话攻击。web 系统的认证通常保存在 session（会话）中，若能攻破系统的会话体系，那么将可以以任意用户身份登录，甚至无需登录，直接访问 web 资源。比如，盗用已登录用户的 cookie、让其他用户基于恶意用户的会话 ID 进行登录、借助已登录用户的状态执行不知情操作（CSRF，跨站请求伪造）。
* 其他常见攻击。一是，密码攻击，基本上就是拿大量密码样本逐一尝试哪个有效，可就这看似毫无技术含量的攻击手法，往往是某些戒备森严环境的罩门所在，因为密码是由用户自行设定的，安全意识薄弱的用户为了便于记忆，通常设定的密码有三个特点，复杂度低（键盘序列，q1w2e3r4）、与个人密切相关（生日，19801231）、所有网站共用相同的账号和密码（支付宝密码与 163 邮箱密码相同），
通常会设定，那么依次对应密码攻击的三种不同手法，暴破、社工、撞库。二是，点击劫持，简单来说，就是在正常页面的上层放置一个透明的恶意页面，用户以为点击的正常页面，其实点击到恶意网站；三是，拒绝服务攻击（DoS），通过让资源耗尽或者服务锁定的方式，让网站无法继续提供访问。

当然，《图解 HTTP》所涉及的知识广度和深度还达不到专业 web 安全人员应具备的基本要求，诸如 web 应用服务器架构、缓存、网关、隧道、代理、字符集、爬虫等等中高阶知识几乎未提及，如果希望系统化深入掌握 HTTP 协议，你需要进入下个阶段，《HTTP 权威指南》。





<div align="center">
<img src="https://github.com/yangyangwithgnu/hanz2piny/blob/master/doc/pics/%E6%9B%BF%E6%8D%A2%E6%97%A0%E6%B3%95%E8%BD%AC%E6%8D%A2%E7%9A%84%E5%AD%97%E7%AC%A6.jpg" alt=""/><br />
（替换无法转换的字符）
</div>


