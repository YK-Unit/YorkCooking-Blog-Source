---
title: 文章模板示例
date: 2020-04-27 12:34:56
categories: ["技术"]
tags: ["2020", "教程"]
comments: true
description: 文章模板详细示例和一些关键细节说明
---

## front-matter

创建文章后，需要在文章头部添加[front-matter](https://hexo.io/docs/front-matter.html)配置信息，`Hexo`才能正确去解析文章的元数据。

`front-matter`示例如下：

```yaml
---
title: #{post-title}            # 文章标题；必须设置
date: YYYY-MM-DD HH:mm:ss       # 文章创建时间；可不设置
categories: ["#{category}"]     # 文章分类数组；可不设置；若设置，一般设置一个
tags: ["#{tag}"]                # 文章标签数组；可不设置
comments: true/false            # 该文章页面是否加载评论；可不设置
description:                    # 文章摘要；可不设置
---
```

注意：

1. 配置使用`YAML`编写
2. 需要保留`---`

> 无注释通用版：
>
> ```YAML
> ---
> title: #{post-title}
> date: YYYY-MM-DD HH:mm:ss
> categories: ["#{category}"]
> tags: ["#{tag}"]
> comments: true
> ---
> ```
>
> 

## config description for post 

设置文章摘要主要有2种方案：

1. 文章中使用` <!-- more --> `手动进行截断（`Hexo` 推荐的方式 ）
2. 在文章的 [front-matter](https://hexo.io/docs/front-matter.html) 中添加 `description`，并提供文章摘录

## image usage example

文章使用本地图片资源的示例如下：

```markdown
![image-usage-example](readme/left-v.jpg)
```

![image-usage-example](readme/left-v.jpg)