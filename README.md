# henland-nftstorage

> NFT-Storage 存储服务接口

## 1、基本信息
该服务通过 NFT-Storage 存储服务；

服务默认监听端口：4444；

文件上传默认限制：100M；

API 接口
- /single
- /multiple

## 2、服务运行

- 修改配置文件
> 1.复制 & 重命名 .env_template 文件 => .env

> 2.配置 .env 文件内的参数

- 运行服务
``` shell
npm install
npm start
```

## 3、服务测试
- 上传单个文件 /single

``` shell
# 请求
curl --request POST \
  --url http://127.0.0.1:4444/single \
  --header 'content-type: multipart/form-data' \
  --form asset=@/Users/lovfer/applications/config/_env/52pojie_1366x768.jpg

# 返回值
{
	"cid": "QmXTEzFxK166HPSFiBm59gQnzdPhXwBmjtNcyrRWR855cn"
}
```

- 上传多个文件 /multiple

``` shell

```

- 查看文件

``` shell

```
