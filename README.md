# fudan_bbs_scraper
复旦大学BBS内容抓取程序 使用说明

一、程序功能
--------------------
本程序由AI生成，供学习、研究和自动化抓取用途。
本程序用于抓取复旦大学 BBS 板块的帖子列表及正文内容，并将结果整理成 Word 文档（.docx）。
支持提取帖子标题、作者、时间、正文以及帖子链接。
程序适用于结构类似的 BBS XML 页面和帖子页面。

二、使用步骤
--------------------
1. 安装依赖
   请确保已安装 Python 3.x，并安装以下依赖库：
   - requests
   - beautifulsoup4
   - python-docx
   可使用以下命令安装：
   pip install requests beautifulsoup4 python-docx

2. 修改板块 URL
   打开程序文件 `你的程序文件.py`，找到以下两行：
   
   BASE_XML_URL = "原来的 XML 链接"
   BASE_ANC_PATH = "原来的路径前缀"
   
   将它们修改为你想抓取的板块对应的 XML 地址和路径前缀，例如：
   
   BASE_XML_URL = "https://bbs.fudan.edu.cn/v18/0an?path=/groups/sport.faq/Running/DACA5FD39/DA14D15FC/D5B8DAE31/DA78613A9/D4F713085"
   BASE_ANC_PATH = "/groups/sport.faq/Running/DACA5FD39/DA14D15FC/D5B8DAE31/DA78613A9/D4F713085"

3. 运行程序
   在命令行中进入程序所在目录，运行：
   python 你的程序文件.py
   程序会依次抓取帖子列表和正文，在命令行中提供复制。

