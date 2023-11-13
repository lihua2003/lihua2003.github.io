 
<head>
    <meta charset="UTF-8">
    <title>机器猫</title>
    <style type="text/css">
        * {
            margin: 0;
            padding: 0;
        }
 
        .whole {
            width: 800px;
            margin: 20px auto;
            /*border: 2px solid yellow;*/
            background-color: white;
            position: relative;
        }
 
        .head {
            margin: 0 auto;
            position: relative;
            width: 500px;
            height: 440px;
            background-color: rgb(0, 183, 231);
            border-radius: 220px;
            border: 1px solid red;
        }
 
        .eye .left_eye,
        .eye .right_eye {
            width: 100px;
            height: 130px;
            background-color: white;
            border: 2px solid black;
            border-radius: 50px;
            position: absolute;
            top: 50px;
            z-index: 3;
        }
 
        .eye .LeyeBall,
        .eye .ReyeBall {
            width: 20px;
            height: 20px;
            background: black;
            border-radius: 10px;
            position: absolute;
            top: 65px;
        }
 
        .eye .left_eye {
            left: 146px;
        }
 
        .eye .right_eye {
            left: 250px;
        }
 
        .eye .LeyeBall {
            right: 10px;
        }
 
        .eye .ReyeBall {
            left: 10px;
        }
 
        .face {
            position: relative;
            z-index: 2;
        }
 
        .face .feature {
            width: 400px;
            height: 320px;
            border-radius: 160px;
            position: absolute;
            top: 100px;
            left: 50px;
            background: white;
        }
 
        .face .nose {
            width: 45px;
            height: 50px;
            border-radius: 23px;
            background-color: rgb(207, 51, 24);
            border: 2px solid black;
            position: absolute;
            top: 165px;
            left: 225px;
            z-index: 3;
        }
 
        .face .Nline {
            width: 3px;
            height: 160px;
            background: black;
            position: absolute;
            top: 218px;
            left: 248px;
            z-index: 3;
        }
 
        .face .mouth {
            width: 280px;
            height: 280px;
            border-bottom: 5px solid black;
            border-radius: 140px;
            position: absolute;
            top: 98px;
            left: 105px;
        }
 
        .face .mustache .MutR_higher {
            width: 80px;
            height: 2px;
            background: black;
            position: absolute;
            top: 220px;
            left: 295px;
            z-index: 2;
        }
 
        .face .mustache .MutR_middle {
            width: 80px;
            height: 2px;
            background: black;
            position: absolute;
            top: 240px;
            left: 295px;
            z-index: 2;
        }
 
        .face .mustache .MutR_lower {
            width: 80px;
            height: 2px;
            background: black;
            position: absolute;
            top: 260px;
            left: 295px;
            z-index: 2;
        }
 
        .face .mustache .MutL_top {
            width: 80px;
            height: 2px;
            background: black;
            position: absolute;
            top: 220px;
            left: 115px;
            z-index: 2;
        }
 
        .face .mustache .MutL_center {
            width: 80px;
            height: 2px;
            background: black;
            position: absolute;
            top: 240px;
            left: 115px;
            z-index: 2;
        }
 
        .face .mustache .MutL_bottom {
            width: 80px;
            height: 2px;
            background: black;
            position: absolute;
            top: 260px;
            left: 115px;
            z-index: 2;
        }
 
        .face .mustache .MutL_bottom,
        .face .mustache .MutR_higher {
            transform: rotate(160deg);
        }
 
        .face .mustache .MutL_top,
        .face .mustache .MutR_lower {
            transform: rotate(200deg);
        }
 
        .neck {
            width: 300px;
            height: 30px;
            background-color: rgb(163, 31, 18);
            border: 2px solid black;
            border-radius: 15px;
            position: relative;
            top: 0px;
            left: 250px;
            z-index: 4;
        }
 
        .neck .bell {
            width: 60px;
            height: 60px;
            overflow: hidden;
            border: 2px solid black;
            border-radius: 60px;
            background-color: rgb(207, 203, 60);
            position: absolute;
            top: 5px;
            left: 120px;
        }
 
        .bell .Bline {
            width: 60px;
            height: 2px;
            background-color: rgb(207, 203, 60);
            border: 2px solid black;
            border-radius: 3px 3px 0 0;
            position: absolut