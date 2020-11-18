# PySitemap

Simple sitemap generator with Python 3

## Description
This is simple and easy sitemap generator written in python which can help you easily create sitemap of your website for SEO and other purposes.

## Options
Simply you can run with thisthis command and program will create sitemap.xml with links from url option
```
python3 main.py --url="https://www.finstead.com"
```

If you want custome path for sitemap file you can add `--output` option like below
```
python3 main.py --url="https://www.finstead.com" --output="/custom/path/sitemap.xml"
python3 main.py --url="http://www.byy3.com" --output="/home/jovyan/guo/PySitemap/sitemap_byy3.com.xml"
python3 main.py --url="http://www.byy3.com" --output="/home/lvwuwei/guo/pysitemap/sitemap_byy3.com.xml"
```
By default program will print parsing urls in console, but if you want to run siletnly you can add `--no-verbose` option. 不显示详解verbose ，在控制台没有任何输出
```
python3 main.py --url="https://www.finstead.com" --output="/custom/path/sitemap.xml" --no-verbose
```

If you want to restrict some urls from being visited by crawler you can exclude them with regex pattern using `--exclude` option. Below code will exclude `png` or `jpg` files.

```
python3 main.py --url="https://www.finstead.com" --output="/custom/path/sitemap.xml" --exclude="\.jpg|\.png"  #排除爬取文件格式
```
