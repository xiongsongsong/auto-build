## build和打包很费人的心思，故尝试一种自动打包方案，缓解这种痛苦

流程大致为：
* 检测combo语法
* 检测是否存在静态文件，文件名像  "a.js,test/abc.js,demo.js"，直接返回
* 如果不存在，则开始进行打包，并生成类似静态文件