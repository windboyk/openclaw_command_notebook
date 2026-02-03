# openclaw避坑指南


## 卸载老版本openclaw
```bash
npm uninstall -g clawdbot moltbot openclaw
```


## 安装最新版的openclaw(老macbook macOS V12.7.6只能使用npm方式安装)

用openclaw的一键安装脚本，会提示不支持v12以下的版本

先去[nodejs官网](https://nodejs.org)下载最新的nodejs进行安装

```bash
npm install -g openclaw@latest
```

## 重新部署openclaw
```bash
openclaw onboard
```

## 重新配置某一项
```bash
openclaw configure
```

## 重新启动openclaw
 ```bash
openclaw gateway restart
``` 

## 给openclaw安装skills(举例安装gemini)
 ```bash
npx clawhub@latest install gemini
```

## 配置好telegram后，需要Pairing
```bash
openclaw pairing approve telegram <Pairing Code>
```
## 启动命令行模式
```bash
openclaw tui
```
## 启动网页端模式
```bash
openclaw dashboard
```
## 设置Chrome扩展的步骤

 1. 安装扩展文件到本地路径：
   ```bash
     openclaw browser extension install
   ```
 2. 获取扩展安装路径：
   ```bash
     openclaw browser extension path
   ```
   这会显示扩展文件所在的目录路径。
 3. 在Chrome中加载扩展：
     - 打开Chrome浏览器
     - 访问 chrome://extensions
     - 启用"开发者模式"
     - 点击"加载已解压的扩展程序"
     - 选择刚才命令输出的目录路径
 4. 固定扩展：
     - 将扩展图标固定到Chrome工具栏上，方便使用

 使用扩展

 - 当你想让OpenClaw控制某个Chrome标签页时，只需点击工具栏上的OpenClaw扩展图标
 - 图标显示"ON"表示该标签页已被OpenClaw控制
 - 再次点击图标可断开连接

 重要注意事项

 - 扩展只控制你主动点击连接的那个标签页，不会自动控制你当前查看的任何标签
 - 这个功能非常强大，相当于让AI代理直接操作你的浏览器，因此建议：
     - 最好使用一个专门的Chrome配置文件（不同于你的个人浏览）
     - 确保OpenClaw网关安全，避免暴露给不信任的网络

 设置完成后，你就可以使用OpenClaw来控制你的Chrome浏览器了。
