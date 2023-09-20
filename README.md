常用的Linux的命令
（01）、echo命令 将指定字符串输出到终端屏幕上
    格式： echo 字符串 或 echo $变量
（02）、date命令 时间命令 
    %t 跳格[Tab键]；%H 小时（00~23）；%I 小时（00~12）；%M分钟（00~59）；%S秒（00~59）；%J 今年中的第几天 
    格式： date 选项 +指定格式
（03）、report命令 重启
（04）、poweroff命令 关机
（05）、wget命令 下载网络文件
    -b后台下载模式 -P下载到指定目录 -t最大尝试次数 -c断点续传 -p下载页面内容所有资源，包括图片和视频 -r递归下载
    格式：wget [参数] 下载地址
（06）、ps命令 查看系统中的进程
    -a显示所有进程（包括其他用户进程）-u用户以及其他详细信息 -x显示没有控制终端的进程
    格式：ps[参数]
（07）、top命令 用于动态的监视进程活动与系统负载等信息
（08）、kill命令 
    终止某个指定PID的进程服务
    格式：kill [参数] [进程PID]
（09）、killall命令
    用于终止某个指定名称的服务多对应的全部进程
    格式：killall [参数] [进程名称]
（10）、ifconfig命令 获取网卡配置与网络状态等信息
    格式：ifconfig [网络设备] [参数]
（11）、uname命令 查看系统内核与系统版本信息
    格式：uname [-a]
（12）、uptime命令 查看系统的负载信息
（13）、free命令 显示当前系统中内存的使用量信息
    格式：free [-h]
（14）、who命令
    查看当前登入主机的用户终端信息
    格式：who[参数]
（15）、last命令
    查看所有系统的登录记录
    格式：last [参数]
（16）、history命令
    显示历史执行过的命令
    格式：histort[-c]
（17）、sosreport命令
    收集系统配置及架构信息并输出诊断文档
（18）、pwd命令
    显示用户当前所处的工作目录
（19）、cd命令
    切换工作路径
    格式：cd [目录名称]；cd- 返回上一次所在的目录；cd.. 进入上级目录； cd~ 切换当前用户的家目录；
        cd~username 切换其他用户的家目录；
（20）、ls命令
    显示目录中的文件信息
    格式：ls [选项] [文件]；-a看全部文件；-l查看文件的属性、大小等详细信息；-d查看目录属性信息
（21）、cat命令
    查看纯文本文件（内容较少的）
    格式：cat [选项] [文件]；-n显示行号
（22）、more命令
    查看纯文本文件（内容较多的）
    格式：more [格式] 文件
（23）、head命令
    查看纯文本文档的前N行
    head [选项] [文件]；例如：输出xxx.cfg文件的前20行；head -n 20 xxx.cfg
（24）、tail命令
    查看纯文本文档的后N行或持续刷新内容
    格式：tail [选项] [文件]；例如：显示前20行：tail -n 20 文件名；显示最新内容：tail -f 文件名
（25）、tr命令
    替换文件名称中的字符
    格式: tr [原始字符] [目标字符]
（26）、wc命令
    统计指定文本的行数、字数、字节数
    格式：wc [参数] 文本；-l只显示行数；-w只显示单词书；-c只显示字节数
（27）、stat命令
    查看存储信息和时间等信息
    格式：stat 文件名称
（28）、cut命令
    按列提取文本字符
    格式：cut [参数] 文本 -f来设置需要看的列数；-d设置间隔符号
（29）、diff命令
    比较多个文本文件的差异
    格式：diff [参数] 文件 --brief确认两个文件是否不同；-c详细比较出多个文件的差异之处
（30）、touch命令
    创建空白文件或设置文件时间
    格式：touch [选项] [文件]；-a仅修改‘读取时间’；-m仅修改‘修改时间’；-d同时修改读取时间和修改时间
（31）、mkdir命令
    创建空白目录
    格式：mkdir [选项] 目录；-p创建具有嵌套关系的文件目录，比如a/b/c/d
（32）、cp命令
    复制文件目录
    格式：cp [选项] 源文件 目标文件；-p保留原始文件的属性；-d若对象为‘链接文件’，则保留该‘链接文件’的属性；
    -r递归持续复制（用于目录）；-i若目标文件存在则询问是否覆盖；-a相当于-pdr（p、d、r为上述参事）
（33）、mv命令
    剪切文件或将文件重命名
    格式：mv [选项] 源文件 [目标路径|目标文件名]
（34）、rm命令
    删除文件或目录
    格式：rm [选线] 文件 -f来强制删除；-r删除文件夹
（35）、dd命令   
    按照指定大小和个数的数据块来复制文件或转换文件
    格式：dd [参数]；if输入的文件名称；of输出的文件名称；bs设置每个‘块’的大小；count设置要复制‘块’的个数
（36）、file命令
    查看文件的类型
    file 文件名
（37）、tar命令
    对文件进行打包压缩或解压
    格式：tar [选项] [文件]；-c创建压缩文件；-x解开压缩文件；-t查看压缩包内有哪些文件；-z用Gzip压缩或解压；
    -j用bzip2压缩或解压；-v显示压缩或解压的压缩；-f目标文件名；-p保留原始的权限与属性；-P使用绝对路径来压缩；
    -C指定解压到的目录
（38）、grep命令
    在文本中执行关键词搜索并显示匹配的结果
    格式：grep [选项] [文件]；-b将可执行文件当做文本文件来搜索；-c仅显示找到的行数；-i忽略大小写；
    -n显示行号；-v反向选择——仅列出没有‘关键词’的行
（39）、find命令
    按照指定条件来查找文件
    格式：find [查找路径] 寻找条件 操作；-name匹配名称；-perm匹配权限；-user匹配所有者；-group匹配所有组
（40）、输入输出重定向
    命令 < 文件                            将文件作为命令的标准输入
    命令 << 分界符                         从标准输入中读入，知道遇见分界符才停止
    命令 < 文件1 > 文件2                   将文件1作为命令的标准输入并将标准输出到文件2
    命令 > 文件                            将标准输出重定向到一个文件中（清空原有文件的数据）
    命令 2> 文件                           将错误输出重定向到一个文件中（清空原有文件的数据）
    命令 >> 文件                           将标准输出重定向到一个文件中（追加到原有内容的后面）
    命令 2>> 文件                          将错误输出重定向到一个文件中（追加到原有内容的后面）
    命令>> 文件 2>&1 或 命令 &>> 文件       将标准输出与错误输出共同写入到文件中（追加到原有内容的后面）
（41）、管道命令符
