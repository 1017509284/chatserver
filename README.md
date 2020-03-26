# chatserver
可以工作在nginx tcp负载均衡环境中的集群聊天服务器和客户端源码 基于muduo实现

# 编译方法1
①cd builb/  
②rm -rf *  
③cmake ..   
④make
# 编译方法2  
./autobuild.sh  
# 各文件的作用  
/include/public.hpp  封装了消息类型的枚举变量    

/include/server/db  封装了数据库层的操作  

/include/server/model 封装了model层的代码，如用户聊天，群组聊天等  

/include/server/redis 封装了redis的发布-订阅操作接口  

/include/server/chatserver.hpp  封装了muduo网络层的主干  

/include/server/chatservice.hpp 封装了所有业务的操作接口  

/src  封装了所有操作接口的实现  

/test 测试代码  

/thirdparty 引用的第三方库json  
