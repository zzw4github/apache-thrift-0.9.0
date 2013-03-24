1实现类及客户端和服务器
src/default package/ 下得三个java类是从D:\thrift-0.9.0\thrift-0.9.0\tutorial\java\src找到的
2两个thrift文件及生成的类 、src/shared  src/tutorial    shared.thrift tutoria.thrift
  这两个文件在tutorial下可以看到
	tutoria.thrift引用了shared.thrift 
	通过   thrift --gen java tutorial.thrift 命令 生成java文件
3 JavaServer类中修改了下面这行
	 params.setKeyStore("D:\\thrift-0.9.0\\thrift-0.9.0\\lib\\java\\test\\.keystore", "thrift", null, null);
	  Use TSSLTransportParameters to setup the required SSL parameters
4.jar包是下载 thrift-0.9.0.tar。gz 解压后 在 lib/java 下运行ant命令生成的