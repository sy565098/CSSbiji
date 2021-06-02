# CSS常用文本样式属性

### color属性
color属性可以设置文本内容的前景色
主要可以用英语单词、十六进制、rgb()、rgba()等表示法
英语单词表示法，比如color：red;仅仅用于学习时临时设置游戏啊颜色，工作时基本不用这样的形式，因为追求精确

### color属性-十六进制表示法
比较常用，时所有涉及软件中都通用的颜色表示法
color：#ff0000;
十六进制ff就是十进制的255，每种颜色分量都是0~255的数字
颜色如果时#aabbcc的形式，可以简写为#abc
黑色时#000，白色时#fff，常见的灰色有#ccc，#333、#2f2f2f等

color属性-rgb()表示法
颜色可以用rgb()表示法
colorL:rgb(255,0,0);

colorshuxing -rgba()表示法
颜色可以用rgba（）表示法，最后一个参数表示透明度，介于0-1之间，0表示纯透明，1表示纯实心
color：rgba（255，0，0，.65）；
rgba()表示法从IE9开始兼容

### font-size属性
用于设置字号，单位通常用px
font-size：30px;
网页文字正文字号通常时16px，浏览器最小支持10px字号

### font-weight属性
font-weight 属性设置字体的粗细程度，通常用normal和bold两个值
font-weight：normal；   正常粗细 与400等值
font-weight：bold;      加粗与700等职
font-weight：lighter    更细，大多数中文字体不支持
font-weight：bolder     更粗，大多数中文字体不支持

### font-style
用于设置字体的倾斜
font-style：normal;        取消倾斜，可以吧天生的i、em等标签设置为不倾斜
font-style：italic;         设置为倾斜字体

### text-decoration
text-decoration 属性用于设置文本的修饰线外观的下划线、删除线
text-decoration：none           没有修饰线
text-decoration：underline;     下划线
text-decoration：line-through;  删除线

### font-family
字体通常时需要已经安装号的字体
定义字体需要根据操作系统和浏览器不同，有eot、woff2、woff、ttf、svg文件格式，需要同时有这5中文件
阿里巴巴普惠体
免费商用授权的普惠字体网址：https：//www.iconfont.cn/webfont

## 继承性
文本相关的属性普遍具有继承性，只需要给祖先标签设置，就可以在后代所有标签中生效
color           font-开头的
list-开头的      text-开头的
line-开头的
因为文字相关属性有继承性，所有通常会设置body标签的字号、颜色、行高等，这样就能当作整个网页的默认样式了

## 课程重点
背诵属性：文字颜色（color）、字体（font-family）、倾斜（font-style：italic）、加粗（font-weight：bold）、下划线（text-decoration:underline）

什么是行高？如何制作单行文本垂直居中
line-height
文字所在一层的高度，文字底部到下一行文字的底部，或者文字顶部到下一行文字的顶部
行高等于盒子高度即可表示文本垂直居中

如何使用font属性快速设置加粗、字号、行高、字体？

课程难点
什么是继承性？哪些属性有继承性？什么是就近原则
css中给祖先设置之后，后代全都有这就是继承性
所有关于文本的都有继承性
在使用继承性的时候，标签的权重暂时失效，这时候看那个选择器近，哪个选择性就继承。
