# 轻量级阿里大鱼扩展包
## 安装
`composer require sentiger/ali-dy -vvv`

## 配置
查看阿里大鱼文档

## 使用
```php
$config    = [
    'accessKeyId'     => 'xxxx',
    'accessKeySecret' => 'xxx',
    'signName'        => 'xxx',
    'templateCode'    => 'xxx',
];
$smsClient = new \Sentiger\AliDy\SMSDy($config);

$res = $smsClient->sendSMS('17602191131', [
    'TemplateParam' => [
        'code' => 'xx'
    ]
]);

print_r($res);
```
