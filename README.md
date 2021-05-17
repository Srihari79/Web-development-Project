# Web-development mini-Project
Abstract: 
This Online Hotel Booking System will help the user to make reservation for hotels online. The user can check the availability of the rooms. The tool provides an option to input start and end dates of the booking. It also takes input such as the number of adults and children. Depending on the availability of the rooms the user can book the room. The user can view the rooms. He can check for different amenities provided by the hotel. The user can also know more about the hotel and its address. Also, we provide pictures of different type of accommodations. This would ease the customer to book rooms. 

 In this project we used HTML, CSS & JS for Front end and 
JAVA for Back end Also, we used Tomcat and Xampp servers 

HTML CODE: 

Index.html : 

<!DOCTYPE html> 

<html> 

<head> 

<meta name="viewport" content="width=device-width, initial-scale=1"> 

<link rel="stylesheet" href="style.css"> 

<h1 style="color:sky blue;text-align:center;" text-align="center">Sky Resorts</h1> 

<style> 

* {box-sizing: border-box} 

body {font-family: Verdana, sans-serif; margin:0} 

.mySlides {display: none} 

img {vertical-align: middle;} 

  

/* Slideshow container */ 

.slideshow-container { 

  max-width: 1000px; 

  position: relative; 

  margin: auto; 

} 

  

/* Next & previous buttons */ 

.prev, .next { 

  cursor: pointer; 

  position: absolute; 

  top: 50%; 

  width: auto; 

  padding: 16px; 

  margin-top: -22px; 

  color: white; 

  font-weight: bold; 

  font-size: 18px; 

  transition: 0.6s ease; 

  border-radius: 0 3px 3px 0; 

  user-select: none; 

} 

  

/* Position the "next button" to the right */ 

.next { 

  right: 0; 

  border-radius: 3px 0 0 3px; 

} 

  

/* On hover, add a black background color with a little bit see-through */ 

.prev:hover, .next:hover { 

  background-color: rgba(0,0,0,0.8); 

} 

  

/* Caption text */ 

.text { 

  color: #f2f2f2; 

  font-size: 15px; 

  padding: 8px 12px; 

  position: absolute; 

  bottom: 8px; 

  width: 100%; 

  text-align: center; 

} 

  

/* Number text (1/3 etc) */ 

.numbertext { 

  color: #f2f2f2; 

  font-size: 12px; 

  padding: 8px 12px; 

  position: absolute; 

  top: 0; 

} 

  

/* The dots/bullets/indicators */ 

.dot { 

  cursor: pointer; 

  height: 15px; 

  width: 15px; 

  margin: 0 2px; 

  background-color: #bbb; 

  border-radius: 50%; 

  display: inline-block; 

  transition: background-color 0.6s ease; 

} 

  

.active, .dot:hover { 

  background-color: #717171; 

} 

  

/* Fading animation */ 

.fade { 

  -webkit-animation-name: fade; 

  -webkit-animation-duration: 1.5s; 

  animation-name: fade; 

  animation-duration: 1.5s; 

} 

  

@-webkit-keyframes fade { 

  from {opacity: .4}  

  to {opacity: 1} 

} 

  

@keyframes fade { 

  from {opacity: .4}  

  to {opacity: 1} 

} 

  

/* On smaller screens, decrease text size */ 

@media only screen and (max-width: 300px) { 

  .prev, .next,.text {font-size: 11px} 

} 

</style> 

</head> 

<body> 

<div class="topnav"> 

  <a class="active" href="index.html">Home</a> 

<a href="booking.html">Book here</a> 

  <a href="aboutusregistration.html">About us</a> 

   <a href="aminitiesregistration.html">Aminities</a> 

   <a href="contactregistration.html">Contact us</a> 

</div> 

<br> 

<br> 

<br> 

<div class="slideshow-container"> 

  

<div class="mySlides fade"> 

  <div class="numbertext">0/ 3</div> 

  <img src="img/sunrise.jpg" style="width:100%"> 

  <div class="text"></div> 

</div> 

  

<div class="mySlides fade"> 

  <div class="numbertext">1 / 3</div> 

  <img src="img/night.jpg" style="width:100%"> 

  <div class="text"></div> 

</div> 

  

  

<div class="mySlides fade"> 

  <div class="numbertext">2 / 3</div> 

  <img src="img/gym.jpg" style="width:100%"> 

  <div class="text"></div> 

</div> 

  

<div class="mySlides fade"> 

  <div class="numbertext">3 / 3</div> 

  <img src="img/dinningimage.jpg" style="width:100%"> 

  <div class="text"></div> 

</div> 

  

<a class="prev" onclick="plusSlides(-1)">&#10094;</a> 

<a class="next" onclick="plusSlides(1)">&#10095;</a> 

  

</div> 

<br> 

  

<div style="text-align:center"> 

  <span class="dot" onclick="currentSlide(1)"></span>  

  <span class="dot" onclick="currentSlide(2)"></span>  

  <span class="dot" onclick="currentSlide(3)"></span>  

</div> 

  

<script> 

var slideIndex = 1; 

showSlides(slideIndex); 

  

function plusSlides(n) { 

  showSlides(slideIndex += n); 

} 

  

function currentSlide(n) { 

  showSlides(slideIndex = n); 

} 

  

function showSlides(n) { 

  var i; 

  var slides = document.getElementsByClassName("mySlides"); 

  var dots = document.getElementsByClassName("dot"); 

  if (n > slides.length) {slideIndex = 1}     

  if (n < 1) {slideIndex = slides.length} 

  for (i = 0; i < slides.length; i++) { 

      slides[i].style.display = "none";   

  } 

  for (i = 0; i < dots.length; i++) { 

      dots[i].className = dots[i].className.replace(" active", ""); 

  } 

  slides[slideIndex-1].style.display = "block";   

  dots[slideIndex-1].className += " active"; 

} 

</script> 

  

</body> 

</html> 

 

 

 

Aboutregistration.html : 

<html> 

<head> 

   <link rel="stylesheet" href="style.css"> 

    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css"> 

    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.5.0/css/bootstrap.min.css"> 

</head> 

<body> 

  <div class="topnav"> 

  <a  href="index.html">Home</a> 

    <a class="active" href="contactregistration.html">Contact us</a> 

   <a href="aminitiesregistration.html">Aminities</a> 

</div> 

<br> 

<br> 

<br> 

  <p> 

       <b> Types of rooms available in out Hotel: 

        there are mainly three types of rooms available in out hotel they are <br> 

        </b> 

  

         

        1)Ac rooms <br> 

        2)Non Ac rooms<br> 

    </p> 

  

    <div class="div1"> 

       <b> <p>1)The Ac rooms </p></b> 

    <p> The  Ac rooms will cost you around 3000 Rs per day, In this  Ac rooms we are  offering the complimentary Breakfast,Bed Tea, News Paper, Internet (wifi & cable), 

         most importantly we allow only 4 members per room</p> 

        <div class="column"> 

          <img src="img/ac.jpg" style="width:198%"> 

        </div> 

       <b> <p> 2)The non Ac rooms </p></b> 

       <p> The Standard Non-AC Rooms Provides you the Economic way of the accommodation. 

            The economic class also gives you the pleasant experience, with greater facilities. 

             These rooms are more spacious laid out neatly with a simple decor give more comfortable. 

              The bathroom is designed more spacious and complete amenities make this room more elegant. 

              The Non Ac Rooms will cost you around 1000 Rs per day, In this Non Ac Rooms there will be no complimentary Breakfast available, most importantly we allow only 4 members per room</p> 

        <div class="column"> 

          <img src="img/nonac.jpg" alt="Forest" style="width:198%"> 

        </div> 

      </div> 

  

</body> 

</html> 

 

amenitiesregistration.html : 

<html> 

<head> 

   <link rel="stylesheet" href="style.css"> 

    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css"> 

    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.5.0/css/bootstrap.min.css"> 

</head> 

<body> 

  <div class="topnav"> 

  <a  class="active" href="index.html">Home</a> 

  <a  href="aboutusregistration.html">About us</a> 

    <a  href="contactregistration.html">Contact us</a> 

</div> 

<br> 

<br> 

<br> 

  <h2> Hotel Amenities</h2> 

  

      <ul> 

  

        <i class="fa fa-clock-o" ></i><li>24-Hour check-in and check-out</li> 

        <i class="fa fa-train"></i><li>10 mins away from Railway Station</li> 

        <i class="fa fa-plane"></i><li>25 mins away from  International Airport</li> 

        <i class="fa fa-coffee"></i><li>Coffee Maker Sachets (Milk, Green Tea, Sugar)</li> 

        <i class="fa fa-wifi"></i><li>Free Wi-Fi</li> 

        <i class="fa fa-briefcase"></i><li>Room service</li> 

        <i class="fa fa-car"></i><li>Free parking</li> 

        <i class="fa fa-wheelchair"></i><li>Wheel Chair Accessibility</li> 

      </ul>   

</body> 

</html> 

 

Booking.html : 

<!DOCTYPE html> 

<html lang="en"> 

<head> 

    <meta charset="UTF-8"> 

    <h1 style="color:solid black;text-align:center;" text-align="center">Register your details</h1> 

    <meta name="viewport" content="width=device-width, initial-scale=1.0"> 

    <link rel="stylesheet" href="style.css"> 

    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css"> 

    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.5.0/css/bootstrap.min.css"> 

    <br> 

    <style> 

           body 

               { 

               background-color:LightBlue 

               } 

</style> 

    

</head> 

<body> 

<div class="topnav"> 

  <a class="active" href="index.html">Home</a> 

  <a href="aboutusregistration.html">About us</a> 

   <a href="aminitiesregistration.html">Aminities</a> 

   <a href="contactregistration.html">Contact us</a> 

</div> 

<br> 

<br> 

<br> 

       <h1 style="color:red;text-align:center;" class="center" ></h1> 

      <form method="post" action="./Registrationservlet"> 

                  <table class="center">     

                       

                        <tr> 

            <td> 

            First Name:</td> 

            <td><input type="text" name="f_name" placeholder="First Name" ></td> 

            </tr>                     

                        <tr> 

            <td> 

            Last Name:</td> 

            <td><input type="text" name="l_name" placeholder="Last Name" ></td> 

            </tr>   

                         <tr> 

            <td> 

            Phone Number</td> 

            <td><input type="text" name="phone" placeholder="Phone Number" ></td> 

            </tr>    

                         <tr> 

            <td> 

            Email</td> 

            <td><input type="email" name="email" placeholder="Email" ></td> 

            </tr>  

                         <tr> 

            <td> 

            From:</td> 

            <td><input type="date" name="from_date" id ="from"  ></td> 

            </tr>  

                        <tr> 

            <td> 

            To:</td> 

            <td><input type="date" name="to_date" id ="to"  ></td> 

            </tr> 

                        <tr> 

                      <td>No of Adults :</td> 

                      <td><select name="adults"> 

                                  <option value="1">1</option> 

                                  <option value="2">2</option> 

                                  <option value="3">3</option> 

                                  <option value="4">4</option> 

                                  <option value="5">5</option> 

                      </select></td> 

                      </tr> 

                      <tr> 

                      <td>No of Children :</td> 

                      <td><select name="children"> 

                                  <option value="1">1</option> 

                                  <option value="2">2</option> 

                                  <option value="3">3</option> 

                                  <option value="4">4</option> 

                                  <option value="5">5</option> 

                      </select></td> 

                      </tr> 

                      <tr> 

                      <td>Preferred Room Type :</td> 

                      <td><select name="room"> 

                                  <option value="AC">Ac</option> 

                                  <option value="NOAC">Non AC</option> 

                      </select></td> 

                      </tr>    

                      <tr> 

                      <td>Preferred Bed Type :</td> 

                      <td><select name="bed"> 

                                  <option value="SingleBedRoom">Single Bed</option> 

                                  <option value="DoubleBedRoom">Double Bed</option> 

                      </select></td> 

                      <tr> 

                      <td style="padding:5px"><input type="submit" name="btn_login" value="Submit"></td> 

                      <td style="padding:5px"><input type="reset" value="Reset"></td> 

                      </tr> 

  

      </form> 

  

</body> 

</html> 

 

Contactregistration.html : 

<html> 

<head> 

   <link rel="stylesheet" href="style.css"> 

    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css"> 

    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.5.0/css/bootstrap.min.css"> 

</head> 

<body> 

<div class="topnav"> 

  <a  href="index.html">Home</a> 

  <a  href="aboutusregistration.html">About us</a> 

   <a  href="aminitiesregistration.html">Aminities</a> 

</div> 

<br> 

<br> 

<br> 

  <nav> 

    <nav> 

      <a href="align=middle tel:6301824577">Contact us : 6301824577</a> 

      <br> 

      <br> 

      <a href="" class="fa fa-linkedin"></a> 

      <a href="" class="fa fa-facebook"></a> 

      <a href="" class="fa fa-twitter"></a> 

      <a href="" class="fa fa-instagram"></a> 

      <a href="" class="fa fa-envelope"></a> 

    

  </nav>  

</nav> 

</body> 

</html> 

 

CSS Code: 

*{ 

    margin: 0; 

    padding: 0; 

} 

body{ 

    border: 2px ; 

  padding: 5px; 

  background: url(file:///C:/Program%20Files/Apache%20Software%20Foundation/Tomcat%209.0/webapps/surya/images/registrationimage.jpg); 

    background-size: top-right; 

  background-repeat: no-repeat; 

  background-size: 2000px 1000px; 

   

} 

  

footer{ 

    border: 2px solid white; 

  padding: 5px; 

  background: url(file:///C:/Program%20Files/Apache%20Software%20Foundation/Tomcat%209.0/webapps/surya/images/registrationimage.jpg); 

    background-size: top-right; 

  background-repeat: no-repeat; 

  background-size: 2000px 1000px; 

  text-align: below; 

} 

  

#form{ 

    background-color: #000; 

    height:400px; 

    width:800px; 

    margin: auto; 

    margin-top: 100px; 

    opacity:0.7; 

} 

#first-group{ 

    border:none; 

    width:400px; 

    margin-top: 38px; 

    position: absolute; 

} 

#content{ 

    border: 1px solid #fff; 

    margin:10px; 

    margin-left: 8px; 

    padding:5px; 

} 

#content #input-group{ 

    border:none; 

    outline:none; 

    background: transparent; 

    margin-left:8px; 

    width:300px; 

    color:#fff; 

} 

::placeholder{ 

    color:#fff; 

} 

.fa{ 

    display:inline-block; 

    color:red; 

    border-right:2px  blue; 

    padding:8px; 

    margin-left: 8px; 

} 

#second-group{ 

    border:none; 

    width:400px; 

    margin-top: 55px; 

    margin-left:200px; 

} 

#submit-btn{ 

    margin-top: 30px; 

    margin-left: 400px; 

    background: transparent; 

    color:#fff; 

    width:150px; 

    border:1px solid red; 

    outline:none; 

    padding:10px; 

    font-size: 20px; 

} 

 

* { 

    box-sizing: border-box; 

  } 

   

  .column { 

    float: bottom; 

    width: 51%; 

    padding: 5px; 

  } 

   

  /* Clearfix (clear floats) */ 

  .row::after { 

    content: ""; 

    clear: both; 

    display: table; 

  } 

  

  h2 ,ul {text-align: center;} 

  

  /* table at center*/ 

  

  .center { 

    margin-left: auto; 

    margin-right: auto; 

    box-align: top; 

  } 

  /* menu bar*/ 

  body { 

  margin: 0; 

  font-family: Arial, Helvetica, sans-serif; 

} 

  

.topnav a { 

  float: left; 

  color: #000; 

  background-color: #000; 

  text-align: center; 

  padding: 14px 16px; 

  text-decoration: none; 

  font-size: 17px; 

} 

  

.topnav a:hover { 

  background-color: #000; 

  color: white; 

} 

  

.topnav a { 

  background-color: #000; 

  color: white; 

} 
