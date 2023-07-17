# ddcheck_plugin
成分姬Yunzai-Bot版本，查询B站关注列表的VTuber/游戏官号成分，并统计成文字发出

VTB列表数据来源：[vtbs.moe](https://vtbs.moe/)

## 使用方式

**更新列表**

```
#更新v列表
```
**查成分**

```
#查成分 B站用户名/UID
```
**注意：首次使用时应该先更新列表，否则本地列表将为空，程序无法对比生成目标成分**

## 部署到云崽

直接部署到 /plugin/example 即可

部署时，请注意控制台载入是否正常，若出现类似“XXX is not defined”的报错，请确认是否安装好对应的依赖

## 配置
请在js内配置您的b站账号的cookie，否在无法查询对象的粉丝牌情况或使用昵称转uid功能（但依然可以通过uid获取其关注列表）

> `cookie` 获取方式：<br>
> 登录bilibili后，`F12` 打开开发工具，查看 `www.bilibili.com` 的请求头下的`cookie`内，形如`buvid3=XXXX;`以及`SESSDATA=XXXX;`的字段，即为您的b站cookie（理论上只要`buvid3`与`SESSDATA`即可，`SESSDATA`可能需要经常更新）

您也可以根据需要配置在js内是否开启自动更新列表，以及自动更新的时间

## 示例
<div align="left">
  <img src="https://i0.hdslb.com/bfs/new_dyn/88a145db1880ccd159e3ea3b48bf524111022578.png" height=500px />
  <img src="https://i0.hdslb.com/bfs/new_dyn/453a037d4108cad14734cadbe48c46b111022578.jpg" height=500px />
</div>

## 其他
### 感谢
* [官方Yunzai-Bot-V3](https://github.com/Le-niao/Yunzai-Bot) : [Gitee](https://gitee.com/Le-niao/Yunzai-Bot)
  / [Github](https://github.com/Le-niao/Yunzai-Bot)
* [noneplugin](https://github.com/noneplugin/) : [NoneBot2 成分姬插件](https://github.com/noneplugin/nonebot-plugin-ddcheck)
