# login_project
<!DOCTYPE HTML>
<html>

<head>
    <title>slick slider</title>
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css"
        integrity="sha384-JcKb8q3iqJ61gNV9KGb8thSsNjpSL0n8PARn9HuZOnIxN0hoP+VmmDGMN5t9UJ0Z" crossorigin="anonymous">
    <link rel="https://cdnjs.cloudflare.com/ajax/libs/slick-carousel/1.8.1/slick-theme.min.css">
    <link="https: //cdnjs.cloudflare.com/ajax/libs/slick-carousel/1.8.1/slick.min.css">
        <style type="text/css">
            body {
                background-color: tomato;
                font-family: lato;
                font-family: sans sarif;
            }
            button:focus{
            outline:none ;
            }
            .form-box {
                width: 380px;
                height: 480px;
                position: relative;
                margin: 6% auto;
                background: #fff;
                padding: 5px;

            }

            .button-box {
                width: 220px;
                margin: 35px auto;
                position: relative;
                box-shadow: 0 0 20px 9px #ff61241f;
                border-radius: 30px;
            }

            .toggle-btn {
                padding: 10px 30px;
                cursor: pointer;
                background: transparent;
                border: 0;
                outline: none;
                position: relative;
            }
            #btn {
                top: 0;
                left: 0;
                position: absolute;
                width: 110px;
                height: 100%;
                background: linear-gradient(to right, #ff105f, #ffad06);
                border-radius: 30px;
                transition: all .5s;
            }

            .social-icons {
                margin: 30px auto;
                text-align: center;
            }

            .social-icons-img {
                width: 30px;
                margin: 0 12px;
                box-shadow: 0 0 20px #7f7f7f3d;
                cursor: Pointer;
                border-radius: 50%;
            }

            .input-group {
                /* top: 180px; */
                position: relative;
                width: 100%;
                transition: .5s;
                text-align: center;
            }

            .input-field {
                margin: 15px 0;
                border-left: 0;
                border-top: 0;
                border-right: 0;
                border-bottom: 1px solid #999;
                outline: none;
                background: transparent;
            }
            .submit-btn {
                width: 85%;
                padding: 10px 30px;
                cursor: pointer;
                display: block;
                margin: auto;
                background: linear-gradient(to right, #ff105f, #ffad06);
                border: 0;
                outline: none;
                border-radius: 30px;
            }

            .check-box {
                position: relative;
                margin-left: -50px;
                margin-bottom: 10px;
            }

            span {
                color: #777;
                font-size: 12px;
                bottom: 68px;
                position: relative;
            }

            #Login {
                display: block;
            }

            #Signin {
                /* left: 450px; */
                display: none;
            }
        </style>
</head>

<body>
    <div class="form-box">
        <div class="button-box">
            <div id="btn"></div>
            <button type="button" class="toggle-btn">Login</button>
            <button type="button" class="toggle-btn">Signin</button>
        </div>
        <div class="social-icons">
            <img src="fb.png">
            <img src="tw.png">
            <img src="gp.png">
        </div>
        <div class="form">
            <form id="Login" class="input-group">
                <input type="text" class="input-field"placeholder="Email Id" required />
                <input type="text" class="input-field" placeholder="Password" required/ >
                <div class="check-box"><input type="checkbox" >Remember Password</div>
                <button type="submit" class="submit-btn">Login</button>
            </form>
            <form id="Signin" class="input-group">
                <input type="text" class="input-field" placeholder="Email Id" required>
                <input type="text" class="input-field" placeholder="Password" required>
                <input type="text" class="input-field" placeholder="Confirm Password" required>
                <div class="check-box"><input type="checkbox" > I agree to this condition</div>
                <button type="submit" class="submit-btn">Login</button>
            </form>
        </div>
    </div>
    <script>
        var x = document.getElementById("Login");
        var y = document.getElementById("Signin");
        var z = document.getElementById("btn");
        var button=document.querySelectorAll(".button-box button");
        button[0].addEventListener("click",()=>{
            x.style.display="block";
            y.style.display="none";
            z.style.left="0";
        })
        button[1].addEventListener("click",()=>{
            x.style.display="none";
            y.style.display="block";
            z.style.left="50%";
        })
        

    </script>
</body>
