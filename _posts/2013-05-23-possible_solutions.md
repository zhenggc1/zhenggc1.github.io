---
layout: post
title: "可能的方案"
description: ""
category: 
tags: [模拟方法]
---
{% include JB/setup %}

# 代理模式

既然是需要对外围调用做模拟，首先想到是从网络层想办法，一个可能的方案就是对jvm加代理

    System.setProperty("socksProxyHost", sockshost);
    System.setProperty("socksProxyPort", sockport);

或者启动的时候添加-D参数，这样，所有外围的交互都会通过这个sock代理，那控制这个代理，也就控制了所有的网路请求，包含请求结果。




# 方法字节码处理
