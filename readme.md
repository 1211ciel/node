My Flag		[l001]
Go		[l002]
Web		[linkWeb]
System		[linkSystem]
English		[linkenglish]
Vim 		[linkVim]

----------------------------------------------------------------------------
My Flag	[l001]
- BookRead v1(ok)
- EnglishStudy v1(ing)
- TimeLine
- Q&A
- WriteBook
- JapaneseStudy
----------------------------------------------------------------------------
Web	[linkWeb]

Js	[linkJs]
Css	[linkCss]

----------------------------------------------------------------------------
Js	[linkJs]

1.计算字符占用的内容 	[js1]

----------------------------------------------------------------------------
计算字符占用的内容 	[js1]
```
    function mbStringLength(s) {
        var totalLength = 0;
        var i;
        var charCode;
        for (i = 0; i < s.length; i++) {
            charCode = s.charCodeAt(i);
            if (charCode < 0x007f) {
                totalLength = totalLength + 1;
            } else if ((0x0080 <= charCode) && (charCode <= 0x07ff)) {
                totalLength += 2;
            } else if ((0x0800 <= charCode) && (charCode <= 0xffff)) {
                totalLength += 3;
            }
        }
        //alert(totalLength);
        return totalLength;
    }

```
----------------------------------------------------------------------------
----------------------------------------------------------------------------
----------------------------------------------------------------------------
Css		[linkCss]

css布局		[linkCssDisplay]
css单位		[linkUnit]
css媒体查询	[linkCssMedia]
css定位		[linkCssPosition]

----------------------------------------------------------------------------
----------------------------------------------------------------------------
----------------------------------------------------------------------------
css布局	[linkCssDisplay]
常见父属性	[linkCss01]
常见子项属性	[linkCss02]

常见父属性	[linkCss01]
flex-direction: 设置主轴方向
	- row 从左到右
	- row-reverse 从右到左
	- column 从上到下
	- column-reverse 从下到上
flex-wrap: 设置元素是否换行
	- nowrap 不换行
	- wrap 换行
justify-content: 设置子元素在主轴上的对齐方式
	- flex-start
	- flex-end
	- center
	- space-around
align-items: 设置子元素在y轴上排列方式（单行）
	- flex-start
	- flex-end
	- center
	- stretch(拉伸)
align-content: 设置子元素在y轴上排列方式（多行）
	- flex-start
	- flex-end
	- space-around
	- space-between
	- stretch



----------------------------------------------------------------------------
常见子项属性	[linkCss02]
flex: 定义子项分配剩余空间
	.item{
		flex:1
	}

align-self: 控制子项在y轴上的排列方式
	- flex-start
	- flex-end
order: 定义项目的排序顺序（数值越小越靠前 默认为0）

----------------------------------------------------------------------------

css单位	[linkUnit]
em	[linkRe]
rem	[linkRem]

----------------------------------------------------------------------------
em	[linkRe]
em 是一个相对单位，相对于父元素的字体大小。
----------------------------------------------------------------------------
rem	[linkRem]
rem（root em)是一个相对单位,相对于html的字体大小。
----------------------------------------------------------------------------
css媒体查询	[linkCssMedia]

@media 可以针对不同的屏幕尺寸设置不同样式
语法
@media mediatype and|not|only (media feature){
	css-code;
}
> mediatype 
	- all 所有设备
	- print 打印机或预览打印
	- scree 电脑屏幕、平板电脑、智能手机
eg:
```
@media screen and (max-width: 800px){
	body:{color:link;}
}

@media screen and (max-width: 500px){
	body:{color:blue;}
}

常见响应式尺寸划分：
- 大屏幕（>=1200px) 设置宽度为 1170px
- 中等屏幕(>=992px) 设置宽度为 970px
- 小屏幕(>=786px)   设置宽度为 750px
- 超小屏幕(<786px)  设置快读为 100%
```

----------------------------------------------------------------------------
css定位	[linkCssPosition]
定位可以让一个元素在盒子内移动，也可以让盒子固定在屏幕的某个位置。
定位模式：
	- static 静态定位（就是标准流）
	- relative 相对定位 相对原来的位置移动，不脱标
	- absolute 绝对定位 相对父元素位置移动，脱标
	- fixed 固定定位 相对于浏览器可视区位置移动，脱标
	- sticky 粘性定位 相对于浏览器可视区位置移动，不脱标，必须加上（top,left,right,bottom 其中一个属性才有效）；当达到属性位置时脱标。
子绝父相：子级使用绝对定位，父级使用相对定位




----------------------------------------------------------------------------
Vim 	[linkVim]
Vim 文件加密解密 	[linkVimEncrypt]

----------------------------------------------------------------------------
Vim 文件加密解密 	[linkVimEncrypt]
```
encrypt
:X
pass
pass

revoke encryption
:x
pass
```
----------------------------------------------------------------------------

