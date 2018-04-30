###1 已经下载模块，导入时却提示找不到，解决方法：
```$xslt
import sys
sys.path.append('模块所在的文件地址')
```
注意：地址中的反斜杠需要加上转义字符，写为“\\”

有的时候依然不管用，可能是因为安装了重复的包需要卸载，最好把whl文件拷贝到project里面来安装

###2 明明有包含需要的对象，却出现错误：
module 'util' has no attribute 'xxx'

原因是module之间互相包含，要改为单向包含
