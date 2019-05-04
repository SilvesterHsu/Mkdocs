# Mkdocs
## readthedocs主题
不支持中文搜索
## material主题
支持中文[搜索](https://squidfunk.github.io/mkdocs-material/getting-started/#site-search)
```
theme:
    name: material #material #readthedocs
    language: 'zh'
extra:
  search:
    language: 'ja'
```
## Docker
可通过Docker进行快速编写，默认自动开启实时反馈
[mkdocs](https://cloud.docker.com/u/silvesterhsu/repository/docker/silvesterhsu/mkdocs)
```
docker pull silvesterhsu/mkdocs:latest
```
```
docker run -v project_PATH:/srv -p 8000:8000 --name project_NAME silvesterhsu/mkdocs:latest /root/init.sh
```
浏览器打开网页，访问 http://127.0.0.1:8000/ 进行预览
