SYNOPSIS

```bash
sed [opts] [cmd chars] [file]
```

Opts

| 参数 | 作用                             |
| ---- | -------------------------------- |
| -n   | 取消默认的sed输出，常与p一起使用 |
| -i   | 修改结果直接写入文件             |
| -e   | 多次编辑（不适用管道符）         |
| -r   | 扩展版正则                       |

内置命令字符

| sed内置         | 作用                               |
| --------------- | ---------------------------------- |
| a               | append，指定行添加一行及以上文本   |
| d               | delete，删除匹配行                 |
| i               | insert，指定行前添加一行及以上文本 |
| p               | print，打印匹配行内容              |
| s/regexp/text/g | 匹配正则内容，替换内容，g全局匹配  |

匹配范围

| 范围      | 解析                              |
| --------- | --------------------------------- |
| 空地址    | 全文处理                          |
| 单地址    | 指定文件某一行                    |
| /pattern/ | 被模式匹配到的每一行              |
| 范围区间  | 10,20 10,+5 /pattern1/,/pattern2/ |
| 步长      | 1~2, 2~2, start~step              |

