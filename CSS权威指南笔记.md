第二章 选择器
    1.基本规则_规则结构
        选择器 + 声明块（一个或多个声明（属性+值(一个关键字或者该属性可取关键字的一个列表（由空格隔开）)））
        h1 {color:red; background:yellow;}
        p {font: medium Helvetica;}
        p {font: large/150% sans-serif;}/* 只有这种情况下使用（/）来分隔两个特定的关键则*/
    2.选择器种类
        元素选择器，类选择器，ID选择器，属性选择器，后代选择器，伪类选择器，伪元素选择器
        
        1.元素选择器
            文档的元素，为最基本的选择器，例如：
            html {color:black;}
            h1 {color:gray;}
            h2 {color:silver;}
        2.选择器分组
            将选择器放在规则的左边，使用逗号分隔。
            h1, p {color:gray;}
        3.通配选择器
            * {color: red;}/*可以让每一个元素都为红色*/
        4.声明分组
            h1 {font: 18px Helvetica; color: purple; background: aqua;}/*注意每个声明后面必须跟（；）*/
        5.结合选择器分组和声明分组
            h1, h2, h3, h4, h5, h6,{color: gray; background: white; padding: 0.5em; border: 1px solid black; forn-family: Charcoal, sans-serif;}
        6.类选择器和ID选择器
            需要适当地标记文档后才能使用这些选择器。
        7.类选择器
            元素需添加class 属性，例如：
            <p class=“warning”>This is a warning paragraph</p>
            *.warning {font-weight: bold;}
            p.warning {font-weight: bold;}
            一个元素可以有多个类中间用空格表示,并且不分顺序。
            <p class="warning urgent">This is a urgent warning paragraph</p>
            .warning.urgent {background: silver} /*同时属于warning和urgent类的元素背景被设置为silver*/
