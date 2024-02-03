# fast-mock-template
🔥 基于 Node.js、 Koa、 Mock.js 的快速搭建 Mock 服务的脚手架项目。

✨ 它旨在为前端开发者提供一个简便、灵活的 Mock 服务，帮助开发者在开发过程中更轻松地模拟接口数据。

## 特性

- 快速搭建：通过简单的配置和命令，快速搭建一个基于 Koa 的 Mock 服务。
- 灵活配置：支持 Mock.js 的强大数据模拟功能，满足各种接口数据需求。
- 易于使用：无需繁琐的配置，简单几步即可启动 Mock 服务，让前端开发更高效。

## 安装

```bash
# 使用 npm 安装
npm install
```

## 使用

1、在 mock 目录下编写 Mock 数据文件，使用 Mock.js 语法进行数据模拟，详细参看 `mock/quickstart.js` 文件。

```
{
  url: '/api/quickstart',
  method: 'get',
  response() {
    return {
      code: 200,
      data: {
        id: Random.id(),
        name: Random.cname()
      }
    }
  }
}
```

2、运行以下命令启动 Mock 服务，并访问 http://localhost:3000/api/quickstart 查看示例。

```bash
npm run dev
```
