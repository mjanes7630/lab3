<!DOCTYPE html>
<html>
    <head>
        <title>Sign Up Page</title>
        
        <!-- JQuery !-->
        <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
        
        <!-- Custom CSS !-->
        <link href="./css/styles.css" rel="stylesheet" type="text/css"/>
        
    </head>
    
    <body>
        
        <h1> Sign Up </h1>
        <br>
        <form id="signupForm" action="welcome.html">
            <div class = "span5"></div>
                <div>
                    <span class="label">First Name :</span>
                    <input type="text" name="fName">
                </div>
                <br>
                <div>
                    <span class="label">Last Name :</span>
                    <input type="text" name="lName">
                </div>
                <br>
                <div>
                    <span class="label">Gender :</span>
                    <input type="radio" name ="gender" value="m"> Male
                    <input type="radio" name="gender" value="f"> Female
                </div>
                <br>
                <div>
                    <span class="label">Zip Code :</span>
                    <input type="text" id="zip" name="zip">
                </div>
                <br>
                <div>
                    <span class="label">City :</span>
                    <span id="city"></span>
                </div>
                <br>
                <div>
                    <span class="label">Latitude :</span>
                    <span id="latitude"></span><br>
                </div>
                <br>
                <div>
                    <span class="label">Longitude :</span>
                    <span id="longitude"></span><br><br>
                </div>
                <div>
                    <span class="label">State :</span>
                    <select id="state" name="state">
                        <option>Select One</option>
                        <option value="ca">California</option>
                        <option value="ny">New York</option>
                        <option value="tx">Texas</option>
                    </select>
                </div>
                <br>
                <div>
                    <span class="label">Select a County :</span>
                    <select id="county"></select>
                </div>
                <br>
                <div>
                    <span class="label">Desired Username :</span>
                    <input type="text" id="username" name="username">
                    <span id="usernameError"></span><br>
                </div>
                <br>
                <div>
                    <span class="label">Password :</span>
                    <input type="password" id="password" name="password">
                </div>
                <br>
                <div>
                    <span class="label">Password Again :</span>
                    <input type="password" id="passwordAgain">
                    <span id="passwordAgainError"></span>
                </div>
                <br>
            </div>
            <input type="submit" value="Sign up!"> 
        </form>
        
        <script>
            
            var usernameAvailable = false;
            //Displaying City from API after typing a zip code
            $("#zip").on("change", async function(){
                
                //alert($("#zip").val());
                let zipCode = $("#zip").val();
                let url = `https://itcdland.csumb.edu/~milara/ajax/cityInfoByZip?zip=${zipCode}`;
                let response = await fetch(url);
                let data = await response.json();
                //console.log(data)
                $("#city").html(data.city);
                $("#latitude").html(data.latitude);
                $("#longitude").html(data.longitude);
                
            });//zip
            
            $("#state").on("change", async function(){
                
                //alert($("#state").val());
                let state = $("#state").val();
                let url = `https://itcdland.csumb.edu/~milara/ajax/countyList.php?state=${state}`
                let response = await fetch(url);
                let data = await response.json();
                //console.log(data);
                $("#county").html("<option> Select One </option>");
                for(let i=0; i < data.length; i++){
                    $("#county").append(`<option> ${data[i].county} </option>`);
                }
                
            });//state
            
            $("#username").on("change", async function(){
                //alert($("#username").val());
                let username = $("#username").val();
                let url = `https://cst336.herokuapp.com/projects/api/usernamesAPI.php?username=${username}`;
                let response = await fetch(url);
                let data = await response.json();
                
                if(data.available){
                    $("#usernameError").html("Username available!");
                    $("#usernameError").css("color", "green");
                    usernameAvailable = true;
                }
                else{
                    $("#usernameError").html("Username not available!");
                    $("#usernameError").css("color", "red");
                    usernameAvailable = false;
                }
            })//username
            
            $("#signupForm").on("submit", function(e){
                //alert("Submitting form...");
                if(!isFormValid()){
                    e.preventDefault();
                }
            });
            
            function isFormValid(){
                isValid = true;
                
                //Username avalibility
                if(!usernameAvailable){
                    isValid = false;
                }
                //Username input
                if($("#username").val().length == 0){
                    isValid = false;
                    $("#usernameError").html("Username is required");
                }
                //Password == Password Again
                if($("#password").val() != $("#passwordAgain").val()){
                    $("#passwordAgainError").html("Password Mismatch!");
                    isValid = false;
                }
                //Password length
                if($("#password").val().length < 6){
                    $("#passwordAgainError").html("Input Six Character Password!");
                    isValid = false;
                }
                return isValid;
            }
        </script>
    </body>
</html>