---
layout:     post
title:      Spring Boot入门学习
subtitle:   自定义banner
date:       2017-10-10
author:     EastLord
header-img: img/post-bg-2015.jpg
catalog: true
tags:
    - Spring Boot
---

# spring boot 自定义banner

#### 项目结构图：

```
├─java
│  └─com
│      └─dongjun
│          └─banner
│              └─demo
│                      Application.java
│                      
└─resources
        application.properties
        banner.txt
```

#### **1.在application.properties添加相关配置:**

```properties
# BANNER   
# Banner file encoding.   

banner.charset=UTF-8   
# Banner file location.   

banner.location=classpath:banner.txt   
# Banner image file location (jpg/png can also be used).    eg:classpath:banner.gif 

banner.image.location=   
# Width of the banner image in chars (default 76)  

banner.image.width=   
# Height of the banner image in chars (default based on image height)  

banner.image.height=   
# Left hand image margin in chars (default 2)   

banner.image.margin=   
# If images should be inverted for dark terminal themes (default false) 

banner.image.invert=   
```

#### **2.在resources目录下创建banner.txt**

spring boot 启动时会自动加载banner.txt

代码：[https://github.com/EastLord/spring-boot-learning](https://github.com/EastLord/spring-boot-learning)

相关网站： [Ascii Art Generator](http://patorjk.com/software/taag) 