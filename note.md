

对于在git上面拉代码报"error: RPC failed; curl 56 OpenSSL SSL_read: SSL_ERROR_SYSCALL, errno 10054"解决方法
是因为git上传文件有限制文件大小，当前上传的文件过大，那么在当前文件执行：
git config http.postBuffer 524288000