# Home Assistant Supervisor

## 首个家庭自动化私有云解决方案

Home Assistant（前身为Hass.io）是一个基于容器的系统，用于管理您的Home Assistant Core安装和相关应用程序。该系统通过与Supervisor通信由Home Assistant进行控制。Supervisor提供了一个API来管理安装。这包括更改网络设置或安装和更新软件。

## 安装

安装说明可在https://home-assistant.io/getting-started找到。

## 开发

对于小的更改和错误修复，您可以直接遵循此步骤，但对于重大更改，请先打开RFC（请求意见书）。开发说明可以在[此处][development]找到。

## 发布

发布分为3个阶段（通道），具有以下结构：

1. 拉取请求合并到“main”分支。
2. 将新构建推送到“dev”阶段。
3. 发布版本。
4. 将新构建推送到“beta”阶段。
5. 更新[`stable.json`][stable]文件。
6. 将推送到“beta”的构建现在将被推送到“stable”。

[development]: https://developers.home-assistant.io/docs/supervisor/development
[stable]: https://github.com/home-assistant/version/blob/master/stable.json