# 如何编辑网站！修改和调整网站内容时，请阅读！

### 文件目录：
- wiki中主要的页面及内容在`pages/`目录下
    - `*.mdx`文件是Wiki页面文件 = HTML <- 一个文件一页wiki
    - `_meta.json`是WIKI页面左侧目录的文件 <- 将文件名转化成汉字或者特定字符显示
    - 和`*.mdx`文件同名的文件夹，用于存放该页面下的子页面

- `theme.config.tsx`是头顶Nav Bar

### 如何更新网站页面及部署
1. 在本地克隆或者在github页面编辑
2. 编辑完成之后，commit至repo的master
3. vercel会自动识别github的repo并重新部署网页

### 注意！
- `pages/`下的文件名请使用小写字母命名
- `_meta.json`的json格式要求

### FAQ
1. commit之后发现网页没有更新？
    - 请等待30秒至1分钟，若还没有更新。
    - 有俩种情况，1. 是vercel抽风导致 2. 代码出现问题导致vercel无法按照最新的commit部署网页 
    - 请找Valor（JianyueHugo）寻求帮助

2. commit之后发现网页左侧目录出现重复内容（英文的文件没有对应中文的内容）？
    - 请检查`_meta.json`文件是否正确编辑，及文件名是否正确。
    - 同时检查github的文件名