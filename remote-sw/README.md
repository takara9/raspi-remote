# ラズパイをGPIO RESTサーバーにするデーモン


これは Raspberry Pi の REST API で操作するためプログラムです。



## インストール方法

OSは、Raspberry Pi OS です。Ubuntuでは確認していません。


```
git clone
sudo make install
```



## REST-APIコール方法

インストールしたpingできるPCなどから、curlでアクセスできます。


GPIO 27 ピンを 300ミリ秒 ONにするには、次のように実行する。

```
curl -X POST http://rp3:8000/api/v1/raspi -H 'Content-Type: application/json'  -d '{"pin":"27","keep":"300"}'
```







