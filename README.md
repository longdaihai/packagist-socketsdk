# hyy websocket API SDK
php websocket

## 安装
```
composer require longdaihai/socketsdk:dev-master
```

## 参考
- hyy_websocket服务端[Gitee下载地址](https://gitee.com/ldh-project/hyy_websocket.git)
## 可调用的方法


## 通用使用教程
### 入口文件
```
require_once './vendor/autoload.php';
```
### 新建一个类继承DingBot
```
use longdaihai\ding\DingBot;

class Dingding extends DingBot
{
    public function __construct()
    {
        parent::__construct([
            'webhook' => 'https://oapi.dingtalk.com/robot/send?access_token=3707d61374a8c4369ddbeae8eedbf93a1772379dee6d75a8f66951e5fc6a8523'
        ]);
    }
}
```
### 使用
```
$ding = new Dingding();
$res = $ding->text("1111111111");
```