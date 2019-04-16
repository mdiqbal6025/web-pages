<!DOCTYPE html>
<html>
<head>
	<meta name="viewport" content="width=device-width, initial-scale=1.0">
	<title>Login page</title>
	<link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css" integrity="sha384-ggOyR0iXCbMQv3Xipma34MD+dH/1fQ784/j6cY/iJTQUOhcWr7x9JvoRxT2MZw1T" crossorigin="anonymous">
	<script src="https://code.jquery.com/jquery-3.3.1.slim.min.js" integrity="sha384-q8i/X+965DzO0rT7abK41JStQIAqVgRVzpbzo5smXKp4YfRvH+8abtTE1Pi6jizo" crossorigin="anonymous"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.14.7/umd/popper.min.js" integrity="sha384-UO2eT0CpHqdSJQ6hJty5KVphtPhzWj9WO1clHTMGa3JDZwrnQq4sF86dIHNDz0W1" crossorigin="anonymous"></script>
<script src="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/js/bootstrap.min.js" integrity="sha384-JjSmVgyd0p3pXB1rRibZUAYoIIy6OrQ6VrjIEaFf/nJGzIxFDsf4x0xIM+B07jRM" crossorigin="anonymous"></script>
<link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.8.1/css/all.css" integrity="sha384-50oBUHEmvpQ+1lW4y57PTFmhCaXp0ML5d60M1M7uH2+nqUivzIebhndOJK28anvf" crossorigin="anonymous">
 <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/animate.css/3.7.0/animate.min.css">
 <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/animate.css/3.7.0/animate.min.css">
<style type="text/css">
	body{
		background:url("D:/New Site/img/2015-HD-Wallpaper.jpg");
		background-size: cover;
		
	}
	.fa-times{
		color:red;
	}
	#wrong{
		visibility: hidden;
		animation-delay: 3s;
		animation-iteration-count: infinite;
		
		
	}
	#rong{
		visibility: hidden;
		animation-delay: 3s;
		animation-iteration-count: infinite;

        
	}
#U,#P{
	color:white;
}
	#para{
		visibility: hidden;
		font-size: 15px;
		color:white;
	}
	#para1{
		visibility: hidden;
		font-size: 15px;
		color:white;
	}
	form{
		background-color: black;
        opacity: 0.8;
        margin-top:200px;
        border-radius:10px;
	}
 button{
 	margin-bottom:10px;
 }
</style>
</head>
<body>
	<script type="text/javascript">
		function check(){
			var x,y;
			x=document.getElementById("user").value;
		    y=document.getElementById("pass").value;
		    if( x=="iqbal" && y=="Hussain"){
		    	
		    	return true;
				
		    }
		     if(x!="iqbal" && y!="Hussain"){
                document.getElementById("U").style.color="red";
                document.getElementById("P").style.color="red";
                 document.getElementById("wrong").style.visibility="visible";
                 document.getElementById("rong").style.visibility="visible";
                 document.getElementById("para").style.visibility="visible";
                 document.getElementById("para1").style.visibility="visible";
		    	return false;
		    }
		    else if(x!="iqbal"){
		    	document.getElementById("U").style.color="red";
                document.getElementById("wrong").style.visibility="visible";
                document.getElementById("para").style.visibility="visible";
		    	return false;
		    }
		    else if(y!="Hussain"){
		    	document.getElementById("P").style.color="red";
		    	document.getElementById("rong").style.visibility="visible";
		    	document.getElementById("para1").style.visibility="visible";
		    	return false;
		    }
		    
		    }
	</script>
 <div class="container">
 	<form action="https://www.google.com" onsubmit="return check()" class="col-md-5 col-lg-4 col-sm-7 mx-auto">
 		<div class="form-group">
 		<label id="U">User Name</label>
 		<input type="text" id="user" class="form-control col-md-8 col-lg-11" placeholder="User Name" required="">
 		<label id="para">Enter correct user name!</label> <i  id="wrong" class="animated zoomIn fas fa-times fa-2x"></i></div>
 		<div class="form-group">
 		<label id="P">Password</label>
 		<input type="password" id="pass" class="form-control col-md-8 col-lg-11" placeholder="Password" required>
	 	<label id="para1">Enter correct Password!</label> <i id="rong" class=" animated zoomIn fas fa-times fa-2x"></i></div>
 		<button type="submit" class="btn btn-success col-lg-3 offset-lg-8 col-sm-4 offset-sm-7">submit</button>
 	</form>
 	
 </div>
</body>
</html>
