# Temp
<?php

session_start();

if(isset($_SESSION['counter']))

{

$_SESSION['counter']+=1;

}

else

{

$_SESSION['counter']=1;

}

$msg = "number of visit to this page is:".$_SESSION['counter'];

$msg .= " in this session.";

?>

<html>

<head>

<title>Setting up a PHP session</title>

</head>

<body>

<?php

echo ($msg);

?>

</body>

</html>
