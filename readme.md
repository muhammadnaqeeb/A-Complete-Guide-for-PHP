<center><h1>PHP Guide</h1></center>

# XAMPP

**XAMPP is the most popular PHP development environment**

XAMPP is a completely free, easy to install Apache distribution containing MariaDB, PHP, and Perl. The XAMPP open source package has been set up to be incredibly easy to install and to use.

1. After installing XAMPP, turn on Apache and mySQL
1. Go to htdocs and create a **folder** there. 
1. Open this folder in VS Code
1. My a php file e g. index.php
1. Go to browser and type localhost/**folder**\_name
1. You serve your first php website

# PHP

Use can write PHP within your HTML syntax using  **<?php ?>**

**PHP is not case sensitive.**
```
<body>
    <div class="container">
        This is my first PHP websites
    </div>
    <?php
      echo "Hello form echo"
    ?>
</body>
```

# Comments in php

### **Single line comments**
```
<?php 
    // This is comment in php
?>
```

### **Multi-line comments**
```
<?php 
/*
P
H
P
*/
?>
```

# New line
```
<?php 
    $var1 = 34;
    $var2 = 45;
    echo "<br>";
    echo $var1;
    echo "<br>";
    echo $var2;
    echo "<br>";
    echo "sum = " , $var1 + $var2;
?>
```
**Output**
```
34
45
sum = 79
```

# Variables
Variable in php starts with **$** sign

In PHP, a variable is declared using a **$ sign** followed by the variable name. Here, some important points to know about variables:

- As PHP is a loosely typed language, so we do not need to declare the data types of the variables. It automatically analyzes the values and makes conversions to its correct datatype.
- After declaring a variable, it can be reused throughout the code.
- Assignment Operator (=) is used to assign the value to a variable.

Syntax of declaring a variable in PHP is given below:

$variablename=value;  
```
<?php 
   $var1 = 34;
   $var2 = 45;
   echo $var1;
   echo $var2;
   echo $var1 + $var2
?>
```


# Arithmetic operator
```
<?php
     $a = 42;
     $b = 20;
     $c = $a + $b;
     echo "Addtion Operation Result: $c <br/>";
     $c = $a - $b;
     echo "Substraction Operation Result: $c <br/>";
     $c = $a \* $b;
     echo "Multiplication Operation Result: $c <br/>";
     $c = $a / $b;
     echo "Division Operation Result: $c <br/>";
     $c = $a % $b;
     echo "Modulus Operation Result: $c <br/>";
     $c = $a++; 
     echo "Increment Operation Result: $c <br/>";
     $c = $a--; 
     echo "Decrement Operation Result: $c <br/>";
?>
```

# Assignment Operator
```
<?php
      $a = 42;
      $b = 20;
      $c = $a + $b;  
      echo "Addtion Operation Result: $c <br/>";
      $c += $a;  
      echo "Add AND Assigment Operation Result: $c <br/>";
      $c -= $a;
      echo "Subtract AND Assignment Operation Result: $c <br/>";
      $c \*= $a; 
      echo "Multiply AND Assignment Operation Result: $c <br/>";
      $c /= $a; 
      echo "Division AND Assignment Operation Result: $c <br/>";
      $c %= $a;
      echo "Modulus AND Assignment Operation Result: $c <br/>";
?>
```
# Comparison Operator
```
<?php
    $x = 25;
    $y = 35;
    $z = "25";
    var_dump($x == $z);  // Outputs: boolean true
    var_dump($x === $z); // Outputs: boolean false
    var_dump($x != $y);  // Outputs: boolean true
    var_dump($x !== $z); // Outputs: boolean true
    var_dump($x < $y);   // Outputs: boolean true
    var_dump($x > $y);   // Outputs: boolean false
    var_dump($x <= $y);  // Outputs: boolean true
    var_dump($x >= $y);  // Outputs: boolean false
?>
```
`var_dump()` function dumps information about one or more variables. The information holds type and value of the variables


# Logical operator
And (&&)

Or( || )

xor

not (!)
```
<?php
   $myvar1 = (true) and (true);
   $myvar2 = (true) && (false);
   $myvar3 = (true) or (false);
   $myvar4 = (true) || (true);
   echo var_dump($myvar1);
   echo var_dump($myvar2);
   echo var_dump($myvar3);
   echo var_dump($myvar4);
?>
```


# Data types

### **String**
```
<?php
  echo "<br>";
  $str = "This is a string";
  echo var\_dump($str);
?>
```
### **Integer** 
```
<?php
echo "<br>";
$in = 45;
echo var\_dump($in);
?>
```

### **Float**
```
<?php
   echo "<br>";
   $fl = 45.258;
   echo var_dump($fl);
?>
```
### **Boolean**
```
<?php
   echo "<br>";
   $boo = True;
   echo var\_dump($boo);
?>
```

# Constant

Constants are like variables except that once they are defined they cannot be changed or undefined.

**define(name, value, case-insensitive)**
```
<?php
   define('PI', 3.14);
   echo PI
?>
```

# If-statement
```
<?php
   $age = 34;
   if($age>18){
       echo "You can go to the party";
   }
   else{
       echo "You can not to the party";
   }
?>
```


# Arrays
Way 1
```
<?php
   $languages = array("Python","PHP","C++");
   echo $languages[0];
   echo count($languages);
?>
```
Way 2
```
$arr = array("one"=>1, "two"=>21);
echo $arr['one'];
echo $arr['two'];
```
# loops

### **while**
```
<?php
   $a = 0;
   while ($a <= 10) {
      echo "<br>The values of  is  : ";
      echo $a ;
      $a++;
   }
?>
```
```
<?php
   $a = 0;
   while ($a < count($languages)) {
      echo "<br> language : ";
      echo $languages[$a];
      $a++;
   }
?>
```
### **Do while**
```
<?php
$a = 0;
do {
    echo "<br>The values of  is  : ";
    echo $a ;
    $a++;
} while ($a < count($languages));
?>
```
### **For**
```
<?php
   for ($a=0; $a <10 ; $a++) { 
       echo "<br> The value of a is: ";
       echo $a;
   }
?>
```
### **Foreach**
```
<?php
   foreach ($languages as $value ) {
      echo "<br>The languge is ";
      echo $value;
   }
?>
```
# Function
```
<?php
   function print5(){
       echo "FIVE";
   }
   print5();
?>
```

```
<?php
function print\_num($num){
    echo "Your number is : ";
    echo $num;
}
print\_num(9999999);
?>
```

# String in PHP

Concatenation is done in php using **.** operator.

### **Length of a string**
```
<?php
   $str ="This is a String";
   $lenn = strlen($str);
   echo "length of a string is : ".$lenn;
?>
```
### **Number of words in string**
```
<?php
   $str ="This is a String";
   echo "  The number of words in this string is : ". str\_word\_count($str)
?>
```
### **Reverse a string**
```
<?php
   $str ="This is a String";
   echo "  The reverse of this string is : ". strrev($str)
?>
```

### **Position of sub-string within string**

```
<?php

$str ="This is a String";

echo "  The position of 'a' in string is : ". strpos($str , "a")

?>
```
### **Replace words in string**
```
<?php
   $str ="This is a String";
   echo "  The replaced string is : ". str\_replace("is" , "at", $str)
?>
```
# Forms
Make a basic form 
```
<form method="post" action="test.php">
      <label for="email">Email</label>
      <br/>
      <input placeholder="Enter Email" type="text" name="emailTB" id="">
      <br/>
      <label for="email">password</label>
      <br/>
      <input placeholder="Enter Password" type="text" name="passwordTB" id="">
      <br/>
      <input type="submit" value="submit">
</form>
```
- PHP receives the data in the $_GET and $_POST arrays
- URL parameters go into the $_GET array
- Data from forms with method="post" do into the $_POST array
- We can check what is the current request method in the $_SERVER array
- Both arrays are global and can be used as any other array
- The name attribute of form input becomes key in the array

### Get data/values of form in test.php
```
<?php 
   $email = $_POST['emailTB'];
   $password = $_POST['passwordTB'];
   echo "Your email is: $email";
   echo "Your password is: $password";
?>
```

# Form with database
Create a database and a table in it in phpmyadmin

![](https://github.com/muhammadnaqeeb/A-Complete-Guide-for-PHP/blob/main/images/002.png)

Create a form in html file
```
<form action="processRecord.php" method="POST">
        Name: <input type="text" name="name" />
        <div></div>
        Registration no: <input type="text" name="RegistrationNo" />
        <div></div>
        <label for="city">Select City</label>
        <select name="cityy" id="cityId">
            <option value="Attock">Attock</option>
            <option value="Islamabad">Islamabad</option>
            <option value="Pindi">Pindi</option>
            <option value="Wah">Wah</option>
        </select>
        <<div></div>
        <label for="">Please select your gender</label>
        <div></div>
        Male <input type="radio" value="Male" name="gender"/>
        Female <input type="radio" value="Female" name="gender"/>
        <div></div>
        <label for="">Hobbies</label>
        <div></div>
         <input type="checkbox" name="hobies[]" value="Sports" name="hobies"/> Sports
         <input type="checkbox" name="hobies[]" value="Music" name="hobies"/> Music
         <input type="checkbox" name="hobies[]" value="Reading" name="hobies"/> Reading
         <div></div>
        <label for="">Please select your favourate color</label>
        <div></div>
        Red <input type="radio" value="Red" name="color"/>
        <div></div>
        Blue <input type="radio" value="Blue" name="color"/>
        <div></div>
        <input value="reset" type="reset">
        <input value="save my record" type="submit">
</form>
```
In php file
```
<!DOCTYPE html>
<html>
<body>
    <?php
    
    // Set connection variables
    $servername = "localhost";
    $username = "root";
    $password = "";
    $dbname = "studentsdb";
    
    // Create connnection
    $conn = mysqli_connect($servername, $username, $password, $dbname);
    
    // Check Connection 
    if(!$conn){
        echo "connection to this database failed due to".mysqli_connect_error();
    }else{
        echo "Success connection to the db";
    }
    
    // collect post variables
    $name = $_POST['name'];
    $RegistrationNo = $_POST['RegistrationNo'];
    
    //city
    $cityy = $_POST['cityy'];
    
    // radio buttons
    $gender = $_POST["gender"];
    
    // checkboxes
    $hobbies = $_POST['hobies'];
    $allHobbies = "";
    foreach ($hobbies as $h){ 
        $allHobbies = $allHobbies . $h;
    }
    
    // radio buttons
    $color = $_POST['color'];
    $sql = "INSERT INTO studentsdb.studentstable VALUES ('$name', '$RegistrationNo','$cityy', '$gender', '$allHobbies', '$color');";
    mysqli_query($conn, $sql);
    ?>
</body>
</html>
```

- $\_SERVER['REQUEST\_METHOD'] holds the name of the request type
- Can be one of 'GET', 'POST', 'HEAD', 'PUT'
- Can be used to detect if user has submitted data or just opens the page from URL
- Case sensitive!

# POST Versus GET


|**GET**|**POST**|
| :-: | :-: |
|In GET method, values are visible in the URL.|In POST method, values are not visible in the URL.|
|GET has a limitation on the length of the values, generally 255 characters.|POST has no limitation on the length of the values since they are submitted via the body of HTTP.|
|This method supports only string data types.|This method supports different data types, such as string, numeric, binary, etc.|
|GET request is often cacheable.|The POST request is hardly cacheable.|
|GET Parameters remain in web browser history.|Parameters are not saved in web browser history.|


# Cookies 

- PHP cookie is a small piece of information which is stored at client browser. It is used to recognize the user.

- Cookie is created at server side and saved to client browser. Each time when client sends request to the server, cookie is embedded with request. Such way, cookie can be received at the server side.

- Each time the same computer requests a page with a browser, it will send the cookie too.

### **Create and Retrieve Cookies With PHP**
A cookie is created with the setcookie() function.

**Syntax**
```
setcookie(name, value, expire, path, domain, secure, httponly);
```
Only the name parameter is required. All other parameters are optional.

**Create PHP Cookies**
```
setcookie($cookie_name, $cookie_value, time() + (86400 * 30), "/"); // 86400 = 1 day
```
**Retrieve a Cookie**
```
$_COOKIE[$cookie_name]
```
`isset()` function to find out if the cookie is set.

**Complete code for cookies**
```
<?php
$cookie_name = "name";
$cookie_value = "Muhammad Naqeeb";
setcookie($cookie_name, $cookie_value, time() + (86400 * 30), "/"); // 86400 = 1 day
?>
<html>
<body>
<?php
if(!isset($\_COOKIE[$cookie\_name])) {
  echo "Cookie named '" . $cookie\_name . "' is not set!";
} else {
  echo "Cookie '" . $cookie\_name . "' is set!<br>";
  echo "Value is: " . $\_COOKIE[$cookie\_name];
}
?>
</body>
</html>
```

**🔑 Note:**

The `setcookie()` function must appear BEFORE the <html> tag.

### **Modify a Cookie Value**
To modify a cookie, just set (again) the cookie using the `setcookie()` function.

### **Delete a Cookie**
To delete a cookie, use the setcookie() function with an expiration date in the past:
```
<?php
   // set the expiration date to one hour ago
   setcookie("user", "", time() - 3600);
?>
<html>
<body>
<?php
   echo "Cookie 'user' is deleted.";
?>
</body>
</html>
```

# Sessions

- A session is a way to store information (in variables) to be used across multiple pages.

- Unlike a cookie, the information is not stored on the users computer.

- Session variables solve this problem by storing user information to be used across multiple pages (e.g. username, favorite color, etc). By default, session variables last until the user closes the browser.
### **Start and Set a PHP Session**
A session is started with the `session_start()` function.

Session variables are set with the PHP global variable: $_SESSION.

```
<?php
   // Start the session
   session_start();
?>
<!DOCTYPE html>
  <html>
   <body>
   <?php
      // Set session variables
      $_SESSION["favcolor"] = "green";
      $_SESSION["favanimal"] = "cat";
      echo "Session variables are set.";
    ?>
    </body>
</html>
```

**🔑 Note:** 

The `session_start()` function must be the very first thing in your document. Before any HTML tags.
### **Get PHP Session Variable Values**
Next, we create another page called "demo_session2.php". From this page, we will access the session information we set on the first page

Notice that session variables are not passed individually to each new page, instead they are retrieved from the session we open at the beginning of each page (session_start()).

Also notice that all session variable values are stored in the global $_SESSION variable:
```
<?php
   session_start();
?>

<!DOCTYPE html>
<html>
  <body>
    <?php
    // Echo session variables that were set on previous page
    echo "Favorite color is " . $_SESSION["favcolor"] . ".<br>";
    echo "Favorite animal is " . $_SESSION["favanimal"] . ".";
    ?>
  </body>
</html>
```
We can also do this
```
<?php
   print_r($_SESSION);
?>
```
### **Modify a PHP Session Variable**
To change a session variable, just overwrite it.

### **Destroy a PHP Session**
To remove all global session variables and destroy the session, use `session_unset()` and `session_destroy()`.
```
<?php
   session_start();
?>

<!DOCTYPE html>
<html>
<body>
<?php
   // remove all session variables
   session_unset();
   // destroy the session
   session_destroy();
?>
</body>
</html>
```
### **Remove certain session data** 

If you want to remove certain session data, simply unset the corresponding key of the $_SESSION associative array, as shown in the following example:
```
<?php 
   // Starting session 
   session_start(); 
   // Removing session data 
   if(isset($_SESSION["lastname"])){ 
   unset($_SESSION["lastname"]); 
} ?> 
```
# session_set_cookie_params

The session_set_cookie_params() is used to set the session cookie parameters defined in the php.ini file.

session_set_cookie_params(seconds) will change the default expiration time of the cookie to what you define.
```
session_set_cookie_params('3600'); // 1 hour

session_set_cookie_params('600'); // 10 minutes.
```
Example:
```
<?php
  $lifetime=600;
  session_set_cookie_params($lifetime);
  session_start();
?>
```
By using session_set_cookie_params, you can define various properties of the session cookie to customize its behavior. Here's a brief explanation of what each parameter does:

**$lifetime:** 

Specifies the lifetime of the session cookie in seconds. By default, the cookie expires when the browser is closed. You can set a specific value to make the cookie last for a longer period, such as a few hours or days.

**$path:** 

Determines the path on the server where the session cookie will be available. If set to '/', the cookie will be available across the entire domain. If set to '/path/', the cookie will only be available within the specified path and its subdirectories. The default value is an empty string, which means the cookie will be available for the current path.

**$domain:** 

Specifies the domain where the session cookie will be available. By default, the cookie is available for the current domain. If you want the cookie to be accessible by subdomains as well, you can set it to 'example.com' instead of 'www.example.com'.


