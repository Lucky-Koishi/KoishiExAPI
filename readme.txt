闭源状态下使用EXAPI之前要做的事情：

1.新建项目；
2.将5个文件拷贝到项目源代码目录下；
3.将项目属性进行如下设置：配置属性→连接器→输入中，忽略特定默认库输入libcmt.lib；
4.附加依赖项中输入koishiex.lib(debug配置下为koishiexd.lib)；
5.在你的代码上面添加#include "koishiex.h"；
6.就可以使用了，但是变量类型前要加命名空间前缀，或者使用using namespace Koishi。