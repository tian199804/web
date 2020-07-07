| 命令行    | 作用                                                         |
| --------- | ------------------------------------------------------------ |
| man       | 查看命令的具体作用例如man ls                                 |
| pwd       | 显示所在路径                                                 |
| cd        | 指定要进入的目录                                             |
| ls        | 列出当前目录的内容                                           |
| rmdir     | 删除空文件夹                                                 |
| rm -f，-r | f强制删除，r递归删除目录及其内容                             |
| touch     | 新建一个文件                                                 |
| cat       | 显示文件内容 cat -n(显示内容和行数)                          |
| vim       | 文本编辑器，按i进入编辑，按esc进入等待命令状态，按:wq保存退出 |
| cp        | 拷贝文件                                                     |
| mv        | 移动文件                                                     |
| open      | 按照系统默认打开程序或文件夹                                 |
| clear     | 清屏，command+k                                              |
| history   | 历史命令查询       history \| grep(关键字搜索)               |
| chmod     | 改变用户操作权限                                             |

# 命令行作业

1. 在document里，新建一个文件夹名字为banyuan
2. 查看document文件夹里的所有文件
3. 进入banyuan文件夹
4. 在banyuan文件夹中，新建一个文件夹 名字为test
5. 进入test文件夹，新建一个文件 banyuan-test.txt
6. 编辑banyuan-test.txt 文件，写入 ‘my first edit’，保存退出。
7. 在test文件夹中，使用默认程序打开banyuan-test.txt 文件
8. 在test文件夹中，创建新的文件夹test1，进入，再创建文件夹test2，进入，打印出当前文件夹路径。
9. 在test2文件夹中，通过**绝对路径**打开banyuan-test.txt 文件。
10. 在test2文件夹中，通过**相对路径**编辑banyuan-test.txt 文件，更改其中内容为‘my second edit’，保存退出。
11. 返回test文件夹，查看banyuan-test.txt的文件内容
12. 改变banyuan-test.txt的权限，使其可读不可编辑
13. 将banyuan-test.txt的权限变回来
14. 查看banyuan-test.txt的内容，显示行数
15. 修改banyuan-test.txt的文件名，改为banyuan-test-edited.txt
16. 退出到document文件夹，删除banyuan文件夹及其中的内容



```shell
 cd Documents
 mkdir banyuan
 ls
 cd banyuan
 mkdir test
 cd test
 touch banyuan-test.txt
 vim banyuan-test.txt
 open banyuan-test.txt
 mkdir test1
 cd test1
 mkdir test2
 cd test2
 pwd
 open /Users/tiantiantian/Documents/banyuan/test/banyuan-test.txt
 vim ../../banyuan-test.txt
 cat banyuan-test.txt
 ls -l
 chmod 444 banyuan-test.txt
 ls -l
 chmod 644 banyuan-test.txt
 ls -l
 cat -n banyuan-test.txt
 mv banyuan-test.txt banyuan-test-edited.txt
 ls
 cd ../../
 rm -r banyuan
 



```

