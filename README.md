# Let'sEncryptSSL证书自动签发脚本

- 安装acme
```bash
curl https://get.acme.sh | sh
```
Or:
```bash
wget -O -  https://get.acme.sh | sh
```

- 打开安装目录
```bash
cd ~/.acme.sh/
```

- 生成域名需要验证的TXT记录
```bash
./acme.sh --issue -d yinhehongbao.com --dns --yes-I-know-dns-manual-mode-enough-go-ahead-please
```

- 配置域名的TXT记录

- 触发验证TXT记录,验证城后生成SSL证书。
```bash
./acme.sh --issue -d yinhehongbao.com --yes-I-know-dns-manual-mode-enough-go-ahead-please
```
