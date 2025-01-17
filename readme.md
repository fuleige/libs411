### 安装

```bash
# 当前目录下执行命令即可
pip install .
```

### 构建包并上传

```shell
# 安装库
pip install build twine

# 构建包上传
# 1. 源码打包构建 (跨平台性好)
pip -m build --sdist
twine upload dist/*

# 2. 构建wheel文件 (需要构建多个平台)
pip -m build --wheel
twine upload dist/*
```