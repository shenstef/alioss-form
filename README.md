laravel-admin extension
======
扩展laravel-admin,web直传阿里OSS（file，image，editor）

### 安装
```
composer require shenstef/alioss-form
php artisan vendor:publish --tag=alioss-form
```
### 配置
新建配置文件config/alioss.php
```
<?php
return [
    'OSS_ACCESS_ID' => '0I********Dx',
    'OSS_ACCESS_KEY' => 'N*******************NT',
    'OSS_ENDPOINT' => 'oss-cn-*****.aliyuncs.com',
    'OSS_BUCKET' => '这里配置BUCKET名',
    'OSS_HOST' => 'http://<BUCKET名>.oss-cn-****.aliyuncs.com',
    //前台显示域名
    'OSS_URL' => 'http://<BUCKET名>.oss-cn-*****.aliyuncs.com', // CDN域名，没有CDN就和OSS_HOST一致即可
];
```

### 使用
```
$form->file('file', '文件');
支持的类型有：
gif,jpeg,jpg,png,bmp,text,txt,doc,docx,ppt,pptx,xls,xlsx,pdf,mp3,wav,aac,flac,avi,mov,flv,mp4,3gp
```

### 截图
![](https://github.com/airan587/alioss-form/blob/master/1.PNG?raw=true)


