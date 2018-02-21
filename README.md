> 文档生成网站的简单代码实例，[预览](http://cnruby.github.io/iotoi/)。将众多[Markdown](http://wowubuntu.com/markdown/)文件快速地生成结构化的网站，并部署至[GitHub](https://github.com)。

## 目录    
- [安装软件](#安装软件)
- [创建项目配置文件](#创建项目配置文件)
- [生成网站实例](#生成网站实例)
- [开发项目代码](#开发项目代码)
- [创建网站GitHub代码库](#创建网站GitHub代码库)
- [部署GitHub](#部署GitHub)

### 安装软件
- 软件网站：[Simpler Paper](https://github.com/DhyanaChina/simpler-paper)
- 运行下面安装命令。

```shell
npm i -g simpler-paper
```

### 创建项目配置文件
- 自动生成配置文件：paper.config.json
- 运行下面命令项目配置文件，在命令执行过程中，需要输入<项目目录>，如本实例目录iotoi_dev。
- 下面命令执行是项目根目录，而不是进入<项目目录>，再执行命令，所有[Simpler Paper](https://github.com/DhyanaChina/simpler-paper)命令都是这样的。

```shell
paper init
```

- 其结果是:

```html  

-------------   项目根目录
|--- iotoi_dev
|    |--- paper.config.json
```

### 生成网站实例
- 自动生成网站实例，其目录为：docs
- 运行下面构建命令：

```shell
paper build
```

> 其结果是:

```html  

-------------   项目根目录
|--- docs
|--- iotoi_dev
|    |--- paper.config.json
```


### 开发项目代码
- 使用网站[Simpler Paper](https://github.com/DhyanaChina/simpler-paper)下的实例代码，或者自己代码
- 使用上面构建命令：

```shell
paper build
```

### 创建网站GitHub代码库
- 创建<GitHub网站目录>，如iotoi
- 使用下面复制命令：

```shell
cp -rf docs/. iotoi/.
```

```html  

-------------   项目根目录
|--- docs
|--- iotoi
|--- iotoi_dev
|    |--- paper.config.json
```

### 部署GitHub
- 将<<项目目录>>和<GitHub网站目录>部署到GitHub上
- 在<GitHub网站目录>代码库上，进入GitHub，登录帐号，菜单Settings，使用GitHub Page。