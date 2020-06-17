//ibm 官网注册创建一个免费的cloud foundry
https://cloud.ibm.com/login

  

//打开ibm官方shell，注意不是容器的ssh

  

`git clone https://github.com/xiaoxiaocer/v2ray-cloudfoundry.git`

`cd v2ray-cloudfoundry/v2ray`

`chmod +x *` 

//你可以自定义修改v2ray的配置文件 config.json

`cd ..`

这里要自己去修改 manifest.yml文件

applications:

\- path: .

  name: GetStartedGo//这里改成你的容器的名称

  random-route: true

  memory: 128M//这里改成你的容器的内存

  

`ibmcloud target --cf`

`ibmcloud cf install`

`ibmcloud cf push`

  

//等待cloud foundry重启成功!


//注册并配置反代
https://dash.cloudflare.com

//workers反代代码为


addEventListener(
"fetch",event => {
let url=new URL(event.request.url);
url.hostname="这里填上面你创建的程序的url（不包含https://）";
let request=new Request(url,event.request);
 event. respondWith(
   fetch(request) 
   ) 
   }
    )

//下载v2使用，如果没有配置id，默认为

'8c35bef3-d51f-41ab-ac87-7b053410495b'
参考配置
vmess://eyJhZGQiOiJjbG91ZGZsYXJlLmNvbSIsImFpZCI6IjY0IiwiaG9zdCI6IuS9oOiHquW3seeahC53b3JrZXJzLmRldiIsImlkIjoiOGMzNWJlZjMtZDUxZi00MWFiLWFjODctN2IwNTM0MTA0OTViIiwibmV0Ijoid3MiLCJwYXRoIjoiIiwicG9ydCI6IjgwODAiLCJwcyI6Ik15IHYyIiwidGxzIjoiIiwidHlwZSI6Im5vbmUiLCJ2IjoiMiJ9

//结束

