步骤一：找到代理地址

<img src='.\img\Snipaste_2026-06-10_19-00-47.png'>

步骤二：仅 GitHub 走代理

```bash
# 协议（二选一）
# socks协议
git config --global http.https://github.com.proxy socks5://127.0.0.1:7897
git config --global https.https://github.com.proxy socks5://127.0.0.1:7897

# 查看
git config --global --get http.https://github.com.proxy

# 不用梯子时删掉
git config --global --unset http.https://github.com.proxy
git config --global --unset https.https://github.com.proxy
```

