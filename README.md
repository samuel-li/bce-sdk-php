# bce-sdk-php
Original respository : https://github.com/baidubce/bce-sdk-php

## Change logs

- [2022-05-09] Replaced the `Guzzle/guzzle` with `GuzzleHttp/guzzle` to support php 7.x.
- [2022-05-10] Support external logger. Example for Laravel: 
```
          \BaiduBce\Log\LogFactory::setInstance(new class(99) implements \BaiduBce\Log\LogFactoryInterface {
                public function getLogger($name) {
                    return Log::channel('chain-baidu');
                }
            }                
        );
        \BaiduBce\Log\LogFactory::setLogLevel(\Psr\Log\LogLevel::INFO);
```



