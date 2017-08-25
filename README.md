# WeChat_forwarding_robot
# 微信转发小机器人 基于 LittleCoder开发的itchat的微信接口 itchat链接 https://github.com/littlecodersh/ItChat

Python练手用的，原理是基于Itchat的网页微信接口来获取消息，判断消息来源转发给另一个微信号。

本来是写给自己用的，所以转发的账号都写死了，后来发现可以通过绑定账号的方式来转发消息

代码比较简单，就不写注释了，只写一下操作方式。

首先你需要一个联网的计算机（我的树莓派还在快递的路上，等到了就放进树莓派里），或者服务器
(我买的阿里云服务器，但是把代码放上去后itchat返回错误，是SSL的问题，我千方百计搞定了SSL认证了https,结果还是那个错误，干脆就部署在本地虚拟机了)

然后你需要一台不用的手机，只要能登微信就好。

将我的代码放在你的服务器或计算机上，然后执行它，会提示你扫描二维码
（我这里的代码是返回一张二维码图片，如果是终端不能显示图片的可以去itchat里有个设置终端生成字符二维码的）

然后手机上确认登录，这时候拿你常用的微信号给这个机器人发送一个绑定消息 #00#bd 
(本来想设置成*#06#的，但是match匹配的时候*是敏感字符。这个梗可能只有上了年纪的人才懂哈哈哈哈哈)

接下来就等别人给你机器人发消息啦

解除绑定使用已绑定的微信号给 机器人发送 #00#quite 就可以解除绑定。

当你的机器人收到别人的消息，会带着对方的姓名转发给你的常用号。

如果你要回复，可以给机器人发送 #你的好友姓名:你要说的话 来回复。

就是这样，很简单！

如果以后还有什么有趣的功能我再加入！
