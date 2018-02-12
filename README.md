# Markdown 練習

## VS Code 擴充功能
1. GFM Preview
1. Markdown PasteURL
1. Markdown Shortcuts

## 標題練習  
\# + space 效果跟\<h1>一樣
\## + space 效果跟\<h2>一樣
\### + space 效果跟\<h3>一樣  
以此類推  

# This is level 1 heading
## This is level 2 heading
### This is level 3 heading

## 換行  
1. 用兩個space + enter換行
1. 用\<br>
1. 用兩個enter換行中間會多空白行

## 字型
1. 粗體 用**包住 or ctrl + B  
Ex: **好粗** 
1. 斜體 用_包住 or ctrl + i  
Ex: _好斜_
1. 刪除線 用~~包住  
Ex: ~~刪掉我~~

## 清單
用 \* + space  
* 安安
* 你好

用 1. + space 做數字清單
1. 清單1  
1. 清單2

用 - [] 做 checkbox 清單
- [ ] list 1  
- [ ] list 2

## 巢狀清單

1. 台灣花蓮周二（6日）晚間23時50分，發生規模6強震，日本媒體同步關心。  
  * 旅居台灣、在花蓮市經營民宿的70歲男子片桐秀明，向《朝日新聞》記者表示，「在台灣住了15年，第一次遇上這麼大的地震」。
 
  * 《朝日新聞》記者於地震後，立刻趕到現場，  
    * 片桐秀明告訴他們：「地震發生時，我在自家三樓睡覺，突然傳來  
    * 『DON! DON! DON! DON!』巨大聲響，伴隨猛烈搖晃，上下晃、左右晃同時發生，到一樓一看，櫃子的抽屜全部飛了出來，桌子也倒了。」
 
2. 片桐又說，當時有6名客人（其中4人是日本人），入住他的民宿，所有人都平安無事。大家躲在一樓一起看電視、關注災情，才知道離民宿約1公里遠的（統帥）飯店1樓，已經整個垮掉。「2天前的深夜，也發生大地震，但今晚的地震搖得更厲害，今年是我在台灣的第15年，第一次遇上這麼大的地震。」

### **注意巢狀清單上限為三層**

## 圖片

### \!\[替代文字](URL "標題")

![騎士湖人交易](https://img.appledaily.com.tw/images/ReNews/20180209/640_336ae59d933d2caf32c14660c70ffb23.jpg "克拉嬸")
美國東岸時間1點13分，騎士先送走明星控衛湯瑪斯(Isaiah Thomas)、老牌射手佛萊(Channing Frye)，以及2018年的受保護首輪選秀，向湖人換來克拉克森(Jordan Clarkson)及南斯(Larry Nance JR)。


![喵喵](https://assets-cdn.github.com/images/modules/open_graph/github-octocat.png)

## 超連結

1. 用 \<> 把 URL 包住  
<https://github.com>

2. 用  \[替代文字](URL "標題")  
[喵咪](https://assets-cdn.github.com/images/modules/open_graph/github-octocat.png "octocat")

1. 用 \[\![圖片替代文字](圖片URL "標題")](URL "標題")  
[![octocat](https://assets-cdn.github.com/images/modules/open_graph/github-octocat.png)](https://github.com/EEITTeam03?tab=repositories)

1. 用 \[自定義名稱]: "URL" 存 URL 再用 \[替代文字][自定義名稱] 顯示

Here is my [HYT git repository][linked]  page

[linked]: https://github.com/EEITTeam03/HY-Tech

## Youtube連結
1. \[\![替代文字](圖片URL)](影片URL)

[![阿明的作文](http://img.youtube.com/vi/bt6b7-ZteJY/0.jpg)](https://youtu.be/bt6b7-ZteJY "Watch video")

## Table

使用 | 切割欄
使用 - 切割標題列

Column A | Column B | Column C
---------|----------|---------
 A1 | B1 | C1
 A2 | B2 | C2
 A3 | B3 | C3

:的位置可讓字往該方想靠

Column D | Column E | Column F
:---------|:----------:|---------:
 D1 | E1 | F1
 D2 | E2 | F2
 D3 | E3 | F3

## 程式區塊

* 用 ``` 包起來

```
public static void Move(int disks, int from, int to)
{
    if(disks == 1)
    {
        System.out.println("Move from " + from + " to " + to);
        return;
    }
     
    int relay = 6 - from - to;
    Move(disks - 1, from, relay);
    Move(1, from, to);
    Move(disks - 1, relay, to);  
} 
```

* 在句子中用 ` 包住程式語法字體會變色

This line has some `alert("Hao")` inline code.

## Emoji

<https://gist.github.com/rxaviers/7360908>

:laughing:  
:blush:
