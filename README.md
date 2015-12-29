# Tag-Web

使用HTML5 Canvas画布绘制标签网（标签云）
use HTML5 Canvas to display a tag web(or tag cloud).

> I'm not very good at English, I'd appreciate if somebody can help me translate this document into English or other language,or you can just point out the mistake,thanks so much.


## Get Start / 开始使用

创建一个DIV元素，并设置ID和宽高
create a div element and set an id and the size.

    <div id="duang" width="400px" height="400px"></div>

然后写JS脚本
then write js

    var obj = new TagWeb("duang");
    //init the tag web
    //初始化标签网
    
    obj.addTag("Tom");
    obj.addTag("Jerry");
    obj.addTag("Andy");
    obj.addTag("Sam");
    ... ...
    //add some tag data
    //添加一些标签数据

Ta-da,it's done.
And you can also see the example.html or other API to learn how to use this.

Duang，您可以看到标签网了。
您也可以查看example.html或者其他接口来了解如何使用本JS库

## Other API / 其他接口

    void init(divID)
    //constructor
    //构造函数
    
    void setLineStyle(strokeStyle)
    //设置线条颜色或样式
    
    void setTextStyle(strokeStyle)
    //设置文字颜色或样式
    
    void setTextFont(fontName)
    //设置字体
    
    void setLineRange(range)
    //if any tag's distance less than the range, it will draw a line between them.
    //设置连线的范围（每个标签间的距离小于该值时连线）
    
    void addTag(tag,fontSize)
    //添加标签
    
    void gridHypodispersion(row,col)
    //it will split the canvas into a grid, and each tag will regeneration with random position in each grid. (>_<)Gee,My English is really bad as shit...
    //网格均匀分布，规定好行列后，重新分布标签位置，使每一个标签在每一个单元格中随机位置
    
    void addCallBack(func)
    //when tag was clicked, it will run this function with a param of tag's content
    //当某个标签被点击后，将会调用func函数，并传递一个为标签内容的参数

## Update Logs / 更新日志
> I think these logs are not very important, so I'm not planing to translate it into other languages.


### ver 0.1.1
2015 / 12 / 29
* 修复标签响应范围的BUG
* 添加压缩后的js库
* 添加gridHypodispersion函数，优化标签分布算法。

## MIT License / MIT协议

enjoy it, thanks.
感谢您的使用。