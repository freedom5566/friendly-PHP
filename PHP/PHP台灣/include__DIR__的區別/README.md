```PHP
include_once __DIR__ ."/ABC.php";
```
和

```PHP
include_once "ABC.php";
```

有甚麼差別？

有人說`echo __DIR__`看看就知道了

返回了`/原生derPHP/PHP台灣/include__DIR__的區別`

[官方文件](http://php.net/manual/en/language.constants.predefined.php "!php.net的ssl怎麼不見惹XD")

不過我打`"../"`或`"./"`通常都沒甚麼問題030

這個問題下去google


`include`跟`require`        
includeb如果文件不存在，會返回警告      
require則會返回錯誤     
加個`_once`可以檢查是否重複引用     
通常靜態標頭都用`require`      
如果需要通過條件判斷則用`include`

上面是已經知道的

我又發現一件好玩的事情

PHP7開始......

`require`也能用在條件判斷裏面了......       
嗯......，這就是為甚麼需要框架RRRRR     
突然想到面試被問，用框架是不是都沒寫到甚麼程式阿

很好很棒，我很期待有新人進去發現一個專案摻雜了幾十個人code style，光這件事情就夠崩潰了吧

沒有統一的規則根本災難