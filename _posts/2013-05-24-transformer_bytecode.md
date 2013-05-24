---
layout: post
title: "转化字节码"
description: ""
category: 
tags: [模拟方法,转化字节码]
---
{% include JB/setup %}

jvm上跑的内容是基于jvm规范来的，不管什么语言，只要可以编译成jvm的指令，就可以在上面跑了，所以现在基于jvm的语言也非常多。

更特殊的，你可以直接编写jvm的字节码。

业界已经提供了很多工具，比如asm，btrace，cglib（基于asm），BCEL等很多类库，并且在jvm启动的时候，也提供了classload的时候来修改class的bytecode。

javaagen的premain方法，提供了Instrumentation的处理，而Instrumentation 则提供了transformer支持。

    public class Main {
        public static void premain(String args, Instrumentation inst) {
            inst.addTransformer(new Transformer());
        }
    }
这个Transformer就可以利用上述的class bytecode工具来修改运行期的bytecode。


