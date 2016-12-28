opencart
========

[OpenCart][1] is designed feature rich, easy to use, search engine
friendly and with a visually appealing interface.

[NTChar][2] is the chinese version of OpenCart.

```
opencart:
  image: jrjang/opencart
  ports:
    - "8000:80"
  links:
    - mysql
  restart: always

mysql:
  image: mysql
  environment:
    - MYSQL_ROOT_PASSWORD=root
    - MYSQL_DATABASE=opencart
  restart: always
```

[1]: http://www.opencart.com/index.php
[2]: http://www.ntcart.com/forum/forum.php
