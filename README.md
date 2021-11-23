## 河南省宗教自动答题脚本，可自定义时间

## [视频教程点击查看](https://gitee.com/zkeq/religious-auto/raw/main/not100.mp4)

### (已更新加密题库)

#### (非官方题库,平均分93 94)

自己写完又校验了一遍,但是还是又很多错误...

校验的时候发现了23个错误,全部改正完之后还是平均分考到93  94 分左右

应该还有18个左右的错误,实在找不出来了......

可以自己去题库里面搜  [不确定]   这个字符,可以看到我不大会做的题

生成题库的项目 : [python提取题库信息自动化脚本](https://github.com/zkeq/religious-auto_data-py)

(自己写的  [题库不大正确,大概90分到95分差不多][没得过80多分,也没超过多95分)

![GIF](https://edu-image.nosdn.127.net/D97468EE8EBE2D04A09C4B76A3F55FE6.gif)

## 本仓库使用方法:

1.下载并解压本仓库到本地

2.本仓库的题库未填正确选项,需要自行修改

3.将题目的答案填入 [extension/js/data.js](/extension/js/data.js) 中的 **answer**中,

  (本步骤已经由本人完成......就是答案正确率不是100%,请看下一步)
  -  (大写字母ABCD) , 
  -  判断题则为正确为A,错误为B. 
  -  多选题不同字母之间**不用**隔任何字符

4.安装脚本,开始使用
  - (在chrome扩展窗口选择安装已经解压的插件,选择**extension**目录即可)

5.快捷提交命令( F12 并打开控制台 输入以下内容): 
  -  ` starttime = '2021-11-XX XX:XX:XX' `即为设置开始时间

  - `autoSubmit()`为提交命令

-------------
-------------
原作者概述:

> 作者：tanyiqu，也就是本人自己
>
> 软件是一个浏览器扩展，安装后点击图标即可使用
> 
> 
> 
> 项目地址：https://github.com/tanyiqu/religious-auto
> 
> 下载：https://github.com/tanyiqu/religious-auto/releases
> 
> 太慢了的话，用网盘链接：https://tanyiqu.lanzoui.com/b0cqofvfe
> 
> **一定对你有用的，请给我的项目点个star**
>
> **仅做学习用途**
> 
> 思路：
> 
> - 使用浏览器扩展方式
> - 注入jquery.js
> - 注入script.js脚本
> - 在script.js中，遍历已有的题库，使用jquery在页面中获取这道题。如果有这道题就把答案选中，没有这道题就跳过
> - 最后点击交卷的时候，系统会自动查找哪道题没有做，最后再做了就行
