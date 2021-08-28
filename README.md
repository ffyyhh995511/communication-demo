# communication-demo
google rpc and protoco buffer

### 1、protocol-buffer是什么
* 协议缓冲区(Protocol Buffers)（Protobufs）像 XML 和 JSON 一样，可以让用不同语言编写并在不同平台上运行的应用程序交换数据。
* 序列化技术,序列化的目的是进行数据存储和交换，依据这个概念，xml,json也是一种序列化的技术  
* XML 和 JSON 相比，Protobuf 编码是二进制而不是文本，这会使调试复杂化

### 2、protocol-buffer使用
* 下载编译工具，本demo下载 [官网](https://github.com/protocolbuffers/protobuf/releases/tag/v3.17.3) protoc-3.17.3-win64.zip，压缩后出现protoc.exe文件,注意maven引入的protobuf-java需要和编译工具同个版本号，demo是3.17.3
* 编写IDL文件*.proto，使用`./protoc --java_out=./my-proto ./my-proto/message.proto` 命令(my-proto是我本地的文件夹)

### 3、protocol-buffer优点
* protocol-buffer是 Google 的语言中立、平台中立、可扩展的结构化数据序列化机制——类似XML，但更小、更快、更简单