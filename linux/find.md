find /opt -name 'pycharm*' # 查找以pycharm开头的文件

find . -name '*.txt'

find . -amin -10 # 查找在系统中最后10分钟访问的文件

find . -atime -2 # 查找在系统中最后48小时访问的文件

find . -[empty()]# 查找在系统中为空的文件或者文件夹

find . -group cat # 查找在系统中属于 groupcat的文件

find . -mmin -5 # 查找在系统中最后5分钟里修改过的文件

find . -mtime -1 #查找在系统中最后24小时里修改过的文件

find . -nouser #查找在系统中属于作废用户的文件

find . -user fred #查找在系统中属于FRED这个用户的文件

find . -type f | xargs grep 'your_string'

find . -type f -name '*.sh' | xargs grep -i 'your_string'