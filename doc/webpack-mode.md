## webpack mode 配置选项

  webpack4之后， 指定webpack需要加载开发环境还是生产环境时，只需要指定mode属性。

  ### 用法

    module.exports = {
      mode: 'development' // production
    }

  或者从cli参数中指定

    webpack --mode development | production

  
  ### 怎样获取当前的运行环境， 需要同时指定 mode

    process.env.NODE_ENV

  | 选项 | 描述 |
  | --- | --- |
  | development| 会将 process.env.NODE_ENV 的值 设定为 development, 启用 NamedChunksPlugin 和 NamedModulesPlugin. |
  | production | 会将 process.env.NODE_ENV 的值 设定为 production |