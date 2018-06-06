#### 连接

```php
//连接数据库
$sql = new mysqli('host','username','password','dbname','port','sockt');
```

#### 执行sql语句

```php
$user = 'root';
$query = "select `host` from user where `user`=?";
$stmt = $sql->prepare($query);

//绑定参数
$stmt->bind_param('s',$user);

//给字段分配变量名称
$stmt->bind_result($host);
$stmt->execute();
```

#### 获取结果

```php
//遍历结果
while($stmt->fetch){
	echo $host;
}
```

