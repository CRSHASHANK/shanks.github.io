<html>
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-9ndCyUaIbzAi2FUVXJi0CjmCapSmO7SnpJef0486qhLnuZ2cdeRhO02iuK6FUUVM" crossorigin="anonymous">
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js" integrity="sha384-geWF76RCwLtnZ8qwWowPQNguL3RmwHVBC9FhGdlKrxdiJJigb/j/68SIy3Te4Bkz" crossorigin="anonymous"></script>
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.7.0/jquery.min.js"></script>
    <style>
        body{
             background-image:url("WMAD/Train.jpeg");
             background-repeat: no-repeat;
             background-size:cover;
             backdrop-filter: blur(3px);
             background-position: center;
            }
        h1{
            font-family:'Lucida Calligraphy';color:darkred;
             text-align: center; text-shadow: 2px 2px 5px lightpink;
             text-decoration:underline black;
        }
        h4{
            font-family:Arial, Helvetica, sans-serif;
            color:blueviolet;
        }
        header{
            background-color:lightgray;
        }
        footer{
            background-color: lightgray;
            text-align: center;
        }
        #r {
        position: relative;
        transition: left 0.5s ease-in-out;
        }
    </style>
    <script>
        $(document).ready(function(){
          $("button").click(function(){
            $("h3").show();
          });
          $("#c").mouseover(function () {
            $("#r").animate({ left: '500px' }, 500); 
        });
        });
        </script>
    <title> HAPPY RAILWAYS</title>
    <link rel="icon" type="img" href="C:\Users\Shalini\Desktop\WMAD\ICON.png">
    <script>
    function validate(){
        var a = document.forms["regform"]["name"].value;
        if (a == "") {
        alert("Full Name must be filled out");
        return false;
        }
        var b = document.forms["regform"]["uname"].value;
        if (b == "") {
        alert("UserName must be filled out");
        return false;
        }
        var c = document.forms["regform"]["age"].value;
        if (c==""){
        alert("Age must be filled out");
        return false; 
        }
        var d = document.forms["regform"]["phno"].value;
        var regno = /^[789]\d{9}$/;
        if (d=="" || !regno.test(d)){
        alert("Valid Mobile Number must be filled out");
        return false; 
        }
        var e = document.forms["regform"]["email"].value;
        var regemail = /^\w+@[a-zA-Z_]+?\.[a-zA-Z]{2,3}$/;
        if (e="" || !regemail.test(e)){
        alert("Valid Email Id must be filled out");
        return false; 
        }
        var f = document.forms["regform"]["gender"].value;
        if (f==false){
        alert("Gender must be filled out");
        return false; 
        }
        var g= document.forms["regform"]["pass"].value;
        var pattern=/(?=.*\d)(?=.*[a-z])(?=.*[A-Z]).{8,20}$/;
        if (g==""){
        alert("Password must be filled out");
        return false; 
        }
        else if(!pattern.test(g)){
        alert("Password is not in required pattern");
        return false; 
        }
        var i = document.forms["regform"]["rpass"].value;
        if (i == "") {
        alert("Re-Enter the Password");
        return false;
        }
        var h= document.getElementById('invalidCheck');
        if (!h.checked){
        alert("Accept the Terms and Conditions");
        return false;
        }
    }
    function toggle(inputId, checkboxId) {
        const inputField = document.getElementById(inputId);
        const checkbox = document.getElementById(checkboxId);
        if (checkbox.checked) {
            inputField.type = 'text';
        } else {
                inputField.type = 'password';
            }
    }  
    function checkPassword() {
        const password = document.getElementById('pass').value;
        const confirmPassword = document.getElementById('rpass').value;
        if (password !== confirmPassword) {
            alert('Password and re-entered password do not match');
        }
    }
    $(document).ready(function(){
    $("#show").click(function(){
    $("p").show();
    });
    });
</script>
</head>
<body><header class="container-fluid"><i><h5> Book Your Train Tickets through Online mode now !!</h5> </i></header>
    <h1><b> Happy Railways </b></h1>
   <a href="C:\Users\Shalini\Desktop\Contact.html" class="link-success"style="float: right; text-decoration-line: none;"><h3>Contact Us</h3></a>
   <h2 style="font-family: Times New Roman; color:darkblue; text-align: center;"><b> Welcome to our Website. Please Sign Up to Continue Ticket Bookings </b></h2>
 <p> <h2 style="text-align: center; color: black;"> Already had an Account? Please login to continue</h2>
<a href="C:\Users\Shalini\Desktop\Login Page.html"  class="link-success" style=" float: right;text-decoration-line: none;"><h3> Log In </h3></a></p>
<img src="C:\Users\Shalini\Desktop\WMAD\Train Logo.png" class="img-thumbnail" height="100" width="100"><br><br>
<button><h2 style="color: darkblue;">Why Happy Railways ?</h2></button><br>
    <h3 style="color:black;display: none;"><br>We are having all the permissions to book Train tickets for Indian Railways.<br>We are also Identified and certified by the Government of India for our long lasting services.<br>
        We are having high security for user data and also provides the user a secure platform to make their payments easy.<br>  
        We offer you amazing discounts and offers on booking tickes throughout the year.</h3><br><br>
      <h2 id="c" style="color: purple;">Check Trains Availability here: </h2><a href="C:\Users\Shalini\Desktop\Availability.html" class="link-success"  style="text-decoration-line: none;"><h2 id="r">  Search Trains  </h2></a><br><br>
<div style="height: 1100px; width: 600px; background-color:rgb(205, 232, 249);border-style: outset;padding:20px;"> 
    <h2 style="color: darkblue;">Registration Form to Sign UP : </h2><br>
<form name="regform" id="Form">
    <h4 style="text-align:justify;">Full Name : <div><input class="form-control form-control-sm" type="text" name="name" placeholder="Enter your Full Name"></div><br>
    Username  : <div class="input-group input-group-sm mb-3">
    <span class="input-group-text" id="inputGroup-sizing-sm">@</span>
    <input type="text" name="uname" class="form-control" placeholder="Enter your Username" aria-describedby="inputGroup-sizing-sm"></div>
    Age       :<div><input class="form-control form-control-sm"name="age" type="number" placeholder="Enter your Age"></div><br>
    Gender    : <div><input type="radio" name="gender" value="Male" required> Male
                   <input type="radio" name="gender" value="Female"> Female </div><br>
    Mobile No : <div><input class="form-control form-control-sm" type="number" name="phno" placeholder="Enter your Mobile Number"></div><br>
    Email ID  : <div><input class="form-control form-control-sm" type="email" name="email" placeholder="Enter your Email Id"></div><br>
    Password  : <div><input class="form-control form-control-sm" type="Password" name="pass" placeholder="Create your Password" id="pass">
    <div class="form-text">
    <h6>*Your password must be 8-20 characters long, contain Uppercase and lowercase letters,numbers, and must not contain spaces or emoji.</h6></div></div>
    <input class="form-check-input" type="checkbox" id="toggle1" onclick="toggle('pass','toggle1')">
    <label class="form-check-label" for="toggle1"><h5 style="color: black;">Show Password</h5></label><br><br>
     Re-Enter Password : <div><input class="form-control form-control-sm" name="rpass" type="password" id="rpass" placeholder="Re-Enter your New Password"></div>
    <input type="checkbox"class="form-check-input" id="toggle2" onclick="toggle('rpass','toggle2')">
    <label class="form-check-label" for="toggle1"><h5 style="color: black;"> Show Password</h5></label><br><br>
    <input class="form-check-input" type="checkbox" id="invalidCheck" name="invalid" onclick="checkPassword()">
    <label class="form-check-label" for="invalidCheck">
    <h5 style="color: green;">Agree to terms and conditions</h5></label>
    <h6> You must agree before submitting.</h6>
    <a class="btn btn-secondary" onclick="return validate()" > Save and Continue </a></h4></form></div><br><br>
<footer class="container-fluid"><i><h5>&copy;2023 Railway Tickets Booking<br>
Followed as per the Rules of Indian Railways</h5>
Feel free to share your comments, suggestions, queries and experiences to us anytime on happyrailways@email.com<br>
Contact us through: 0823-156-3578 </i></footer>
</body>
</html>


<html>
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-9ndCyUaIbzAi2FUVXJi0CjmCapSmO7SnpJef0486qhLnuZ2cdeRhO02iuK6FUUVM" crossorigin="anonymous">
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js" integrity="sha384-geWF76RCwLtnZ8qwWowPQNguL3RmwHVBC9FhGdlKrxdiJJigb/j/68SIy3Te4Bkz" crossorigin="anonymous"></script>
    <script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
    <style>
    h1{
        text-align:center; color:darkblue;
        border-style: outset; border-color: darkgreen; 
        background-color:lavender;
        text-shadow: 2px 2px 5px lightgreen ;
        font-family: 'Lucida Calligraphy';
    }
    header{
        background-color:lightgray;
    }
    footer{
        background-color: lightgray;
        text-align: center;
    }
</style>
<title> HAPPY RAILWAYS</title>
<link rel="icon" type="img" href="C:\Users\Shalini\Desktop\WMAD\ICON.png">
<script>
    $(document).ready(function(){
        $("#btnToggle").click(function(){
            $("#p1").fadeIn();
            $("#p2").fadeIn("slow");
        });
        $("h3").mouseover(function(){
            $("#s").css("color", "green")
      .slideUp(2000)
      .slideDown(2000);
    });
});
</script>
</head>
<body style="background-color: snow;">
    <header class="container-fluid"><i><h5> Book Your Train Tickets through Online mode now !!</h5> </i></header>
    <h1><b>Happy Railways</b></h1>
    <a  class="link-success" style="text-align: center; text-decoration-line: none;" href="C:\Users\Shalini\Desktop\Online Railway Booking.html" ><h3 > HOME </h3></a>
    <img src="C:\Users\Shalini\Desktop\WMAD\Train Logo.png" class="img-thumbnail" height="100" width="100">
    <div id="d1" style="margin: 0 auto;border:outset green;width:600px;height:500px;padding:20px;"><h3 style="color: purple;">CONTACT: </h3><p id="s" style="display: none;">ONE STOP SHOP FOR ALL TRAIN TRAVEL</p><br><br>
    <h5>* Contact us directly on happyrailways@email.com.<br>
    * All Train tickets beyond India.<br>
    * Always the most cost effective and convinient connection.<br></h5><br>
    <button id="btnToggle">Full Details</button><br><br>
    <p id="p1" style="display:none;"><b>Opening Hours:</b><br>
    Monday to Friday:- 09:00 am to 06:00pm</p><br>
    <p id="p2" style="display:none;"><b>Head Quarters:-</b><br>Soumya Palace,<br>K.R Puram main Street,<br>Banglore.</p></div><br><br>
    <footer class="container-fluid"><i><h5>&copy;2023 Railway Tickets Booking<br>
        Followed as per the Rules of Indian Railways</h5>
        Feel free to share your comments, suggestions, queries and experiences to us anytime on happyrailways@email.com<br>
        Contact us through: 0823-156-3578 </i></footer>  
</body>
</html>


<html>
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-9ndCyUaIbzAi2FUVXJi0CjmCapSmO7SnpJef0486qhLnuZ2cdeRhO02iuK6FUUVM" crossorigin="anonymous">
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js" integrity="sha384-geWF76RCwLtnZ8qwWowPQNguL3RmwHVBC9FhGdlKrxdiJJigb/j/68SIy3Te4Bkz" crossorigin="anonymous"></script>
    <style>
    h1{
        text-align:center; color:darkblue;
        border-style: outset; border-color: darkgreen; 
        background-color:lavender;
        text-shadow: 2px 2px 5px lightgreen ;
        font-family: 'Lucida Calligraphy';
    }
    h4{
      font-family: 'Times New Roman';
      color:purple;
    }
    header{
        background-color:lightgray;
    }
    footer{
        background-color: lightgray;
        text-align: center;
    }
</style>
<title> HAPPY RAILWAYS</title>
<link rel="icon" type="img" href="C:\Users\Shalini\Desktop\WMAD\ICON.png">
<script>
    function validate(){
        var a = document.forms["login"]["uname"].value;
        if (a == "") {
        alert("Username must be filled out");
        return false;
        }
        var b = document.forms["login"]["pass"].value;
        var pattern=/(?=.*\d)(?=.*[a-z])(?=.*[A-Z]).{8,20}$/;
        if (b == "") {
        alert("Password must be filled out");
        return false;
        }
        else if(!pattern.test(b)){
        alert("Password is not in required pattern");
        return false; 
        }
    
}
</script>
</head>
<body style="background-color: snow;">
    <header class="container-fluid"><i><h5> Book Your Train Tickets through Online mode now !!</h5> </i></header>
    <h1><b>Happy Railways</b></h1>
    <div class="container text-center">
        <div class="row">
            <div class="column">
                <a  class="link-success" href="C:\Users\Shalini\Desktop\Online Railway Booking.html"><h3 > HOME </h3></a>
            </div>
        </div>
    </div>
    <img src="C:\Users\Shalini\Desktop\WMAD\Train Logo.png" class="img-thumbnail" height="100" width="100"  >
    <h2 style="color: darkred; text-align: center; font-family: Verdana;" > Log In into your Account</h2><br>
    <form name="login">
   <div style="width:500px;height:400px;margin: 0 auto;border:outset green;padding:20px;"><br>
    <h4> USERNAME: <div><input class="form-control form-control-sm" type="text" name="uname" size="30" placeholder="Enter your Username">
    </div><br>
    PASSWORD: <div><input class="form-control form-control-sm" type="password" size="30" name="pass" placeholder="Enter your Password"></h4><br>
    <a class="btn btn-secondary" onclick="validate()">Log In</a><br><br>
    <div class="alert alert-warning" role="alert">
        Give the data which is used while signing up!!
    </div></div>
    </form><br><br>
    <footer class="container-fluid"><i><h5>&copy;2023 Railway Tickets Booking<br>
        Followed as per the Rules of Indian Railways</h5>
        Feel free to share your comments, suggestions, queries and experiences to us anytime on happyrailways@email.com<br>
        Contact us through: 0823-156-3578 </i></footer>
</body>
</html>


<html>
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-9ndCyUaIbzAi2FUVXJi0CjmCapSmO7SnpJef0486qhLnuZ2cdeRhO02iuK6FUUVM" crossorigin="anonymous">
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js" integrity="sha384-geWF76RCwLtnZ8qwWowPQNguL3RmwHVBC9FhGdlKrxdiJJigb/j/68SIy3Te4Bkz" crossorigin="anonymous"></script>
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.7.0/jquery.min.js"></script>
    <style>
    h1{
        text-align:center; color:darkblue;
        border-style: outset; border-color: darkgreen; 
        background-color:lavender;
        text-shadow: 2px 2px 5px lightgreen ;
        font-family: 'Lucida Calligraphy';
    }
    h4{
        font-family:'Times New Roman';
        color:purple;
    }
    body{
        background-color:snow;
    }
    header{
            background-color:lightgray;
        }	
    footer{
            background-color: lightgray;
            text-align: center;
        }
    </style>
    <script>
     $(document).ready(function(){
  $("#b1").click(function(){
    $("#p1").toggle()
  }); 
    $("#b2").click(function() {
            $("#2").slideDown();
            $("#2").animate({fontSize: '2em'}, "slow");
});
});
    </script>
    <title> HAPPY RAILWAYS</title>
    <link rel="icon" type="img" href="C:\Users\Shalini\Desktop\WMAD\ICON.png">
</head>
<body>
    <header class="container-fluid"><i><h5> Book Your Train Tickets through Online mode now !!</h5> </i></header>
   <h1><b>Happy Railways</b></h1>
   <div class="container text-center">
    <div class="row">
      <div class="col">
        <a  class="link-success" href="C:\Users\Shalini\Desktop\Online Railway Booking.html" style="text-decoration-line: none;"><h3 > HOME </h3></a>
      </div>
      <div class="col">
        <a  class="link-success" href="C:\Users\Shalini\Desktop\Login Page.html" style="text-decoration-line: none;"><h3 > LOG IN </h3></a>
      </div>
    </div>
   </div>
   <img src="C:\Users\Shalini\Desktop\WMAD\Train Logo.png" class="img-thumbnail" height="100" width="100" style="float: left;"  ><br><br>
   <h2 style="color: darkred; text-align: center; font-family: Verdana;" > Enter the Details below to Search the Trains </h2><br>
   <button id="b1" style="margin: 0 auto; display: block; padding-left: 10px;padding-right: 10px;">NOTE</button><br>
   <p id="p1" style="display: none; color:blue; text-align: center;" >You can book tickets only for 4 persons at single time </p>
   <form>
    <div id="1" style="width: 500px; height: 800px; margin: 0 auto;border: outset green;padding:20px;">
        <h4>SOURCE :<div><input class="form-control form-control-sm" type="text" placeholder="Enter Source" required></div><br>
        DESTINATION :<div><input class="form-control form-control-sm" type="text" placeholder="Enter Destination" required></div><br>
        DATE :<div><input class="form-control form-control-sm" type="date" required ></div><br>
        CLASS :<div><input class="form-control form-control-sm" list="classes" id="class" placeholder="Select Class" required>
        <datalist id="classes">
            <option value ="First Class">
            <option value ="Second Class">
            <option value ="Third Class">
            <option value="Chair Car">    
            <option value ="Second Sitting">  
        </datalist></div><br>
        TYPE :<div><input type="radio" name="1" value="NON AC" required> NON AC
              <input type="radio" name="1" value="AC"> AC</div><br>
        QUOTA :<div><input class="form-control form-control-sm" list="quota" id="Quota" placeholder="Select Quota" required>
        <datalist id="quota">
        <option value ="General">
        <option value ="Ladies">
        <option value ="Tathkal">
        <option value="Person with Disablility">
        <option value ="Senior Citizen">         
        </datalist></div><br>
        NO OF PASSENGERS :<div><input class="form-control form-control-sm" type="number" placeholder="Enter No of Passengers" required></div><br>
        <button type="button" id="b2" class="btn btn-secondary">Check Availability</button></h4>
        <div id="2" class="alert alert-info " role="alert" style="display: none;">
            Information Submitted !!
        </div>
        </div></form> <br>
        <footer class="container-fluid" ><i><h5>2023 Railway Tickets Booking<br>
            Followed as per the Rules of Indian Railways</h5>
            Feel free to share your comments, suggestions, queries and experiences to us anytime on happyrailways@email.com<br>
            Contact us through: 0823-156-3578 </i></footer>
</body>
</html>

