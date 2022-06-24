
## 致谢

 **（1）字体**

- chncwk - [屏显臻宋 Clear Han Serif](https://www.maoken.com/freefonts/3329.html)

 **（2）工具**

- fontTools - [pyftsubset](https://fonttools.readthedocs.io/en/latest/subset/) & [ttLib.woff2](https://fonttools.readthedocs.io/en/latest/index.html?highlight=ttLib.woff2#utilities)

- 夜煞之乐2001(NightFurySL2001) - [字体计数软件 CJK-character-count](https://github.com/NightFurySL2001/CJK-character-count)

 **（3）字表**

- 《通用规范汉字表》（8105字）

- GB2312 中的汉字（6763字）

  注：额外添加了“〇”。



## 用法

 **（1）文件列表**

```
/* TTF 格式 */
/ttf/clearhanserif.original.v1.07.ttf
/ttf/clearhanserif.subset.v1.07.gb2312.ttf
/ttf/clearhanserif.subset.v1.07.standard.ttf

/* WOFF2 格式 */
/woff2/clearhanserif.subset.v1.07.standard.woff2
/woff2/clearhanserif.original.v1.07.woff2
/woff2/clearhanserif.subset.v1.07.gb2312.woff2

/* 字表 */
/text/gb2312.txt
/text/standard.txt
```

 **（2）文件名**

- 文件名含 `original` 的是 @chncwk 发布的未子集化的源文件

- 文件名含 `subset` 的是子集化后的文件

- 文件名含 `gb2312` 的字体使用了 GB2312 字库精简

- 文件名含 `standard` 的字体使用了《通用规范汉字表》精简


 **（3）使用**

若要在网页中将该字体用作 WebFont （建议使用 WOFF2 格式），

可在样式表中如此调用：

```css
@font-face {
  font-family: Clear Han Serif;
  font-display: swap;
  src:  local(Clear Han Serif),
        url("/fonts/clearhanserif.subset.v1.07.gb2312.woff2") format("woff2");
}
        /* 浏览器会首先检查本地是否已安装该字体，
           若否，则会从网站根目录的 fonts 文件夹中加载 */

body {
  font-family: Clear Han Serif, system-ui, -apple-system, BlinkMacSystemFont, sans-serif, serif;
}
```



## 其他

[前往 npm](https://www.npmjs.com/package/clear-han-serif-subset)
