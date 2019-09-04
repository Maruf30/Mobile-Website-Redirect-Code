# Mobile-Website-Redirect-Code




<?php
$iphone = strpos($_SERVER['HTTP_USER_AGENT'],"iPhone");
$android = strpos($_SERVER['HTTP_USER_AGENT'],"Android");
$palmpre = strpos($_SERVER['HTTP_USER_AGENT'],"webOS");
$berry = strpos($_SERVER['HTTP_USER_AGENT'],"BlackBerry");
$ipod = strpos($_SERVER['HTTP_USER_AGENT'],"iPod");
 
if ($iphone || $android || $palmpre || $ipod || $berry == true) 
{
    echo "<script>window.location='http://m.site.com'</script>";
 }
?>


Note: Works when added to the header.php file in most WordPress themes.
Or
Using a JavaScript code you can redirect your mobile visitors to your mobile site. This JS code can either detect screen size or the user-agent.




<script type="text/javascript">
  <!--
  if (screen.width <= 800) {
    window.location = "http://m.domain.com";
  }
  //-->
</script>
