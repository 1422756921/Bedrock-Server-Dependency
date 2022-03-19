# 基岩版服务器依赖
Minecraft 基岩版服务器 (Centos 或者其他 Linux) 依赖包

# 为什么要使用这个依赖？
因为 Mojang 只提供对 Ubuntu 的支持，所以不能在其他系统（Centos 等）上支持

出于这个原因，我从 Ubuntu 中提取了必要的依赖项
并将它们放在 Bedrock 服务器上，以便它们可以在除 Ubuntu 以外的系统上执行

# 食用教程
1.找到你的服务器目录
<pre><code>cd /yourserver
</code></pre>

2.下载依赖
<pre><code>wget https://github.com/1422756921/Bedrock-Server-Dependency/raw/main/pack.tar.gz
</code></pre>

3.解压依赖包
<pre><code>tar -zvxf pack.tar.gz
</code></pre>

4.使用此命令打开您的服务器
<pre><code>LD_PRELOAD= ./ld-linux-x86-64.so.2 --inhibit-cache --library-path . ./bedrock_server
</code></pre>
