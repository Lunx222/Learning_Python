已经下载模块，导入时却提示找不到，解决方法：
```$xslt
import sys
sys.path.append('模块所在的文件地址')
```
注意：地址中的反斜杠需要加上转义字符，写为“\\”