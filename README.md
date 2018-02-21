> 文档生成网站的简单代码实例. [预览](http://cnruby.github.io/iotoi/)。将众多 Markdown 文件快速地生成结构化的网站，并部署至GitHub。

## 目录    
- [安装软件](#安装软件)
- [创建项目配置文件](#创建项目配置文件)
- [生成网站实例](#生成网站实例)
- [开发项目代码](#开发项目代码)
- [创建网站GitHub代码库](#创建网站GitHub代码库)
- [部署GitHub](#部署GitHub)

### 创建实例
- 进入网站：[Simpler Paper](https://github.com/DhyanaChina/simpler-paper)
- 运行下面安装命令。

```shell
npm i -g simpler-paper
```

### 创建项目配置文件
- 自动生成配置文件：paper.config.json
- 运行下面命令项目配置文件，在命令执行过程中，需要输入<项目目录>，如本实例目录iotoi_dev。
- 下面命令执行目录是项目目录，而不是进入下面项目目录，再执行命令，所有paper命令都是这样的。

```shell
paper init
```

- 其结果是:

```html  

-------------   project dir
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

-------------   project dir
|--- docs
|--- iotoi_dev
|    |--- paper.config.json
```


### 开发项目代码
- 使用网站[Simpler Paper](https://github.com/DhyanaChina/simpler-paper)下的实例
- 使用上面构建命令

```shell
paper build
```

### 创建网站GitHub代码库
- 创建<GitHub网站目录>，如iotoi
- 使用命令：

```shell
cp -rf docs/. iotoi/.
```

```html  

-------------   project dir
|--- docs
|--- iotoi
|--- iotoi_dev
|    |--- paper.config.json
```

### 部署GitHub
- 将<<项目目录>>和<GitHub网站目录>部署到GitHub上
- 在<GitHub网站目录>代码库上，进入GitHub，登录帐号，菜单Settings，使用GitHub Page。