<h1 align="center"> EasyWeChat Console Tool </h1>

<p align="center">A command line for EasyWeChat Application.</p>

## Installing

```shell
$ composer require easywechat/console -vvv
```

Or install it globally:

```shell
$ composer global require easywechat/console -vvv
```

## Usage

```shell
$ ./vendor/bin/easywechat list

# globally install
$ easywechat list
```

### Get payment RSA public key.

https://pay.weixin.qq.com/wiki/doc/api/tools/mch_pay.php?chapter=24_7

```shell
$ ./vendor/bin/easywechat payment:rsa_public_key \
    --mch_id=14339221228 \
    --api_key=36YTbDmLgyQ52noqdxgwGiYy \
    --cert_path=/Users/overtrue/www/demo/apiclient_cert.pem \
    --key_path=/Users/overtrue/www/demo/apiclient_key.pem 
    
# Public key of mch_id:14339221228 saved as ./public-14339221228.pem
```

## License

MIT