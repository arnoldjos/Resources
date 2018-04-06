Database Functions
==================

Connect to database
-------------------
```sh
mysqli_connect(server, user, password, database_name);
```

Perform queries to database
---------------------------
```sh
mysqli_query($connection, $query);
```

Fetch row from database as associative array
--------------------------------------------
```sh
myqli_fetch_assoc($result_from_mysqli_query);
```

Fetch row from database as array
--------------------------------------------
```sh
myqli_fetch_array($result_from_mysqli_query);
```

Other Functions
===============

Check if variable is set
------------------------
```sh
isset();
```

Security Functions
==================

Protect against sql injection
-----------------------------
```sh
mysqli_real_escape_string($connection, $data_to_protect);
```

Encrypt data
------------
```sh
$hashformat = "$2y$10$";
$salt = "iusesomecrazystrings2$";
$hashformat .= $salt;

crypt($data_to_encrypt, $hashFormat);
```
