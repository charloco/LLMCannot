# 背景
现在需要将client机器的某个目录共享给server,计划如此实现
1. 在server运行fuseserver
2. 在client运行fuseclient
3. 当fuseclient连接到fuseserver后, fuseserver会自动mount一个/mnt/share目录
4. /mnt/share目录下读取,创建,删除,写入等操作通通过client的tcp连接传给client,client对具体文件操作
5. 使用github.com/hanwen/go-fuse
上面的代码就是按照这个要求提供server的规划和具体golang代码

# 结果

试过了很多LLM，都没有有效的完成
