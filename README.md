### 世邦英文及西芝英文商务通代码

因为公司经常性的更改网站联系信息及商务通信息，导致技术人员疲于应付此类诸多事情，鉴于此，有必要统一规范下大家的网页代码书写规范。

规范如下：
1. 一个网站下只引用一个商务通js文件，不可把代码内联到网页中，需要外部引用，由于网站周期一般不会超过很多年，强烈建议个人所属下的网站，都引用一个外部js文件，比如你的网站全是西芝的，你只需要在第一个网站建立一个js文件，比如livechat.js，以后所有的网站都引用此商务通代码文件，http://www.yourfirstdoamin.com/livechat.js 
2. 网页中的电话邮箱，最好要用js替换方式，或者在所有电话及邮箱前后加上注释，以便未来可以批量修改

---
简介：

## 商务通JS代码说明 

**声明:** 通过在商务通代码前后添加注释标识，可以在以后更换商务通代码通过正则规则匹配来批量替换商务通代码。

**注意：**js文件中的代码注释不要去掉，压缩文件时请检查 。


### 世邦商务通代码

```JavaScript
//#@+livechat-sbm-content
document.write('<script src="http://pkt.zoosnet.net/JS/LsJS.aspx?siteid=PKT56764896&float=1&lng=en"><\/script>');   
//#@-livechat-sbm-content
```

### 西芝商务通代码

```JavaScript
//#@+livechat-zenith-content
document.write('<script src="http://pkt.zoosnet.net/JS/LsJS.aspx?siteid=PKT21646611&float=1&lng=en"><\/script>');   
//#@-livechat-zenith-content
```

### 中文商务通代码【与世邦的一样】

```JavaScript
//#@+cnlivechat-sbm-content
document.write('<script src="http://pkt.zoosnet.net/JS/LsJS.aspx?siteid=PKT56764896&float=1&lng=en"><\/script>');   
//#@-cnlivechat-sbm-content
```
**说明：**
> //#@+ 与 #@- 用于标识这其中的内容，可以使用sed命令批量替换之中的内容，但为了区分不同的品牌与不同的所属人，需要加上公司名标识与个人名字标识。如果以后再更换商务能，可以在VPS下，通过find命令批量替换世邦的商务通，或者批量替换西芝的商务通。也可以通过脚本，批量替换某个人的商务通代码。比如通过zhanglei这个标识，可以批量替换只属于zhanglei的网站。 后面那个名字是可选的，只要有前面的唯一标识，就可以批量替换了。

## 留言板代码说明

仍然强烈建议使用统一的模板文件来显示留言板，可以外链到js文件中，如果你不想这样使用，务必按按照以下操作

留言板代码前后需要加上注释，如下：
```Html
<!--Start Message Board-->
...你的留言板代码....
<!--End Message Board-->
```

建议所有的留言板都换成引用js文件方式 ，和上面的商务能代码一样，可以批量替换的，因为留言板在以后必定会换的。你统一放进一个js文件里，可以在以后的工作中节省很多时间。 因为留言板代码，不同的人可能会有不同的代码风格，所以建议在最后加上自己的名字，<!--Start Message Board Style1-->

##  联系信息说明 【待】
```Html
<li>Address:B-32, 4th floor, Ekta, Opp. fire brigade office. Near Oberoi mall. Goregaon (E). Mumbai-63 </li>
<li>Tel:+91-9076003100/+91-9928911119</li>
<li>Contact Person:Vijay Kumar/Kerry</li>
<li>E-mail: info@zenithcrusher.com </li>
```

```Html
<li>Address: <!--Start Zentih Address--> B-32, 4th floor, Ekta, Opp. fire brigade office. Near Oberoi mall. Goregaon (E). Mumbai-63 <!--End Zenith Address--></li>
<li>Tel:<!--Start Zentih Telphone-->+91-9076003100/+91-9928911119<!--End Zenith Telphone--></li>
<li>Contact Person:Vijay Kumar/Kerry</li>
<li>E-mail:  <!--Start Zentih Email-->info@zenithcrusher.com<!--End Zenith Email--></li>
```

## 记住
你自己不同网站之间共有的东西，一定要是代码风格与内容一致的，这样可以批量替换，如果担心对SEO有影响，可以使用JS替换技术，目前这块只能靠自己做，因为还没有人花精力做这块事情。商务通，电话，邮箱，留言板，这些几乎每年都会更改一次，或者几次，以上所有的建议都是让大家可以方便在未来发生更改时及时快速的更改自己的网站，而不再费心费思的。

### 附注

By @Ray - [love4026.org](http://love4026.org/)