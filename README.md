Encrypt data with aes 128 and 256 byte
And decrypt it in Codeigniter

## Example :

```
<?php
define('BASEPATH',__DIR__);
if (!file_exists('AES.php')) {
    copy('https://raw.githubusercontent.com/mm4130/encrypt-decrypt-php-codeigniter/master/AES.php', 'AES.php');
}
require_once __DIR__.'/AES.php';
$xm = new AES('aes',128);
//Encrypt
$enc = $xm->encrypt('data','password');
echo $enc;
//Decrypt
echo $xm->Decrypt($enc,'password');
?>
```
## For AES 256
```
<?php
define('BASEPATH',__DIR__);
if (!file_exists('AES.php')) {
    copy('https://raw.githubusercontent.com/mm4130/encrypt-decrypt-php-codeigniter/master/AES.php', 'AES.php');
}
require_once __DIR__.'/AES.php';
$xm = new AES();
//Encrypt
$enc = $xm->encrypt('data','password');
echo $enc;
//Decrypt
echo $xm->Decrypt($enc,'password');
?>
```
