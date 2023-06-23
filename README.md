# 一个有点六的论文搜刮器：pda (parse dblp abstract)

应用场景：你导让你搜刮近年来的论文，你可以提取出几个关键词，但却要一个一个地确认论文摘要内容是否符合你的要求，这个时候，pda就派上用场了。

此工具有如下功能：

1. 通过dblp来搜索论文，可以设置标题、venue、年份或仅搜索期刊。
2. 爬取每一篇论文摘要内容。(此功能需要 chromedriver 支持)
3. 使用AI来决策论文是否与关键词符合，如果符合则采用更加精炼的语言介绍论文内容，不符合则删除。(需要配置ChatGPT API)
4. 将论文收集结果导出为Markdown的表格，可以复制它到任意表格软件中。
5. 导出搜集论文的BibTex信息，生成`.bib`文件，可以直接在论文中引用。

## Install

```shell
pip3 install parseDblpAbstract -U
```

## Usage

```shell
pda
```
