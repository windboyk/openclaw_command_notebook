# openclaw避坑指南
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

## 卸载openclaw
```bash
npm uninstall -g clawdbot moltbot openclaw
```

## 配置好telegram后，需要Pairing
```bash
openclaw pairing approve telegram <Pairing Code>
```

## 安装最新版的openclaw(老macbook macOS V12.7.6只能使用npm方式安装)
用openclaw的一键安装脚本，会提示不支持v12以下的版本
去[nodejs官网](https://nodejs.org)下载最新的nodejs进行安装
```bash
npm install -g openclaw@latest
```
