#ufile sdk
base on https://docs.ucloud.cn/api/ufile-api/index 
#usage
```php
    $sdk = new UfileSdk('storage','api_pub_key','api_pub_secret');
    $sdk->put('text.txt',"content");
    $sdk->putFile('text.txt',"/path/to/yourfile");
    $contents = $sdk->get('dd');
    $exists = $sdk->exists('dd222');
    $size = $sdk->delete('dd');
```
或者直接查看tests/sdkTest.php