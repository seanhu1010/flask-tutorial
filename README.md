# Flaskr
Flask [教程](http://flask.pocoo.org/docs/tutorial/)基本博客应用程序

## 安装项目

**请务必使用与您正在阅读的文档版本相同的代码版本。**

```
#克隆存储库
#复制打包的软件包到任意目录
cd flask-tutorial
```

在Windows cmd中，创建virtualenv并激活它：
```
python3 -m venv venv
. venv/bin/activate
```

安装软件包 Flaskr:

```
pip install -e .
```

## 运行软件

在Windows cmd中:

```
set FLASK_APP=flaskr
set FLASK_ENV=development
flask init-db #初始化数据库
flask run
```

打开网址[http://127.0.0.1:5000](http://127.0.0.1:5000/)

## 测试

```
pip install '.[test]'
pytest
```

运行覆盖率报告：

```
coverage run -m pytest
coverage report
coverage html  # 在浏览器中打开htmlcov/index.html
```

