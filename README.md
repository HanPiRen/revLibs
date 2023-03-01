# RevLib Support for QChatGPT

得益于[QChatGPT项目](https://github.com/RockChinQ/QChatGPT)的插件功能，此插件将允许接入`ChatGPT网页版`用以替换原项目主线的GPT-3模型接口，提升回复质量。  
[官方接口与ChatGPT网页版的区别？](https://github.com/RockChinQ/QChatGPT/wiki/%E5%AE%98%E6%96%B9%E6%8E%A5%E5%8F%A3%E4%B8%8EChatGPT%E7%BD%91%E9%A1%B5%E7%89%88)

## 使用方式

> 若您未安装QChatGPT程序，请先查看原仓库[文档](https://github.com/RockChinQ/QChatGPT)  
> 目前已支持中国主机使用，请在revcfg.py中修改openai_account字段，按照注释使用access_token方式登录

使用管理员账号私聊机器人发送指令:

```
!plugin https://github.com/RockChinQ/revLibs
```

若无法访问GitHub，可以使用Gitee镜像

```
!plugin https://gitee.com/RockChin/revLibs
```

等待程序获取源码，并解决依赖，这可能需要数分钟的时间。  
安装完毕后，请发送:
```
!reload
```
重载插件，生成配置文件，**关闭主程序**。  
到`QChatGPT`程序目录编辑`revcfg.py`文件，根据注释修改必填配置项。  
配置完成后重新启动主程序以使用。

### **❗注意：由于此接口响应较慢，请在主程序`config.py`中将`process_message_timeout`字段设置为300以上**