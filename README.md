<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="utf-8">
    <title>Html5 - 小猫咪</title>
    <link rel="stylesheet" type="text/css" href="css/common/reset.css"/>
    <style>
        body{text-align: center;}
        .wrapper{ height:800px;}
        canvas{ margin-top: 123px;}
    </style>
</head>
<body>
    <div class="wrapper">
        <canvas width="600" height="554"></canvas>
    </div>

    <script>
        var cvs=document.querySelector("canvas");
        var g=cvs.getContext("2d");
        
        //尾巴
        g.strokeStyle="#33190c";
        g.fillStyle="#ffffd9";
        g.lineWidth=6;
        g.beginPath();
          g.moveTo(433,458);
          g.lineTo(477,438);
          g.bezierCurveTo(492,433,496,453,484,463);
          g.lineTo(433,494);
        g.fill();
        g.stroke();

        //身体
        g.beginPath();
          g.moveTo(255,392);
          g.lineTo(255,526);
          g.bezierCurveTo(256,555,282,557,293,530);
          g.lineTo(383,530);
          g.bezierCurveTo(392,557,419,558,428,526);
          g.quadraticCurveTo(434,523,430,393);
        g.closePath();
        g.fill();
        g.stroke();
        //肚白
        g.fillStyle="#fff";
        g.beginPath();
          g.moveTo(317,501);
          g.quadraticCurveTo(345,504,363,500);
          g.quadraticCurveTo(386,492,389,480);
          g.quadraticCurveTo(393,469,396,437);
        g.closePath();
        g.fill();
        //肚子蓝点
        g.fillStyle="#e5f8ef";
        g.beginPath();
          g.moveTo(428,459);
          g.bezierCurveTo(407,456,405,479,421,482);
          g.bezierCurveTo(393,482,394,507,427,511);
          g.quadraticCurveTo(429,485,428,459);
        g.closePath();
        g.fill();

        //耳朵(左边)
        g.strokeStyle="#33190c";
        g.fillStyle="#ffffd9";
        g.lineWidth=4;
        g.beginPath();
          g.moveTo(106,79);
          g.quadraticCurveTo(114,4,209,14);
        g.fill();
        g.stroke();
        //耳朵(右边)
        g.beginPath();
          g.lineWidth=5;
          g.moveTo(376,14);
          g.quadraticCurveTo(431,13,446,15);
          g.quadraticCurveTo(488,20,498,48);
          g.quadraticCurveTo(508,75,512,110);
        g.fill();
        g.stroke();

        g.beginPath();
          g.lineWidth=8;
          g.moveTo(470,65);
          g.lineTo(483,27);
        g.stroke();

        g.beginPath();
          g.fillStyle="#fecce5";
          g.moveTo(473,65);
          g.lineTo(483,30);
          g.bezierCurveTo(502,46,496,60,512,110);
        g.closePath();
        g.fill();

        //头
        g.lineWidth=10;
        g.beginPath();
          g.strokeStyle="#33190c";
          g.fillStyle="#ffffd9";
          g.moveTo(280,6);
          g.bezierCurveTo(476,0,535,154,541,166);
          g.lineTo(546,180);
          g.bezierCurveTo(584,304,530,368,432,392);
          g.quadraticCurveTo(210,460,90,372);
          g.quadraticCurveTo(38,324,34,314);
          g.quadraticCurveTo(1,268,38,174);
          g.quadraticCurveTo(128,8,280,6);
        g.closePath();
        g.fill();
        g.stroke();

        //脸白
        g.fillStyle="#fff";
        g.beginPath();
          g.moveTo(29,294);
          g.quadraticCurveTo(57,339,99,371);
          g.quadraticCurveTo(272,404,427,390);
          g.bezierCurveTo(500,371,567,330,549,216);
          g.bezierCurveTo(560,298,518,360,427,378);
          g.quadraticCurveTo(272,404,99,364);
          g.quadraticCurveTo(55,334,29,294);
        g.closePath();
        g.fill();

        //胡须(左边)
        g.strokeStyle="#33190c";
        g.lineWidth=7;
        g.beginPath();
          g.moveTo(6,212);
          g.lineTo(23,212);
          g.stroke();
          g.moveTo(7,211);
          g.quadraticCurveTo(5,212,7,213);
        g.stroke();

        g.beginPath();
          g.moveTo(2,246);
          g.lineTo(15,246);
          g.stroke();
          g.moveTo(6,245);
          g.quadraticCurveTo(1,246,6,247);
        g.stroke();

        g.beginPath();
          g.moveTo(6,284);
          g.lineTo(17,281);
          g.stroke();
          g.moveTo(9,282);
          g.quadraticCurveTo(4,287,6,282);
        g.stroke();
        //胡须(右边边)
        g.lineWidth=6;
        g.beginPath();
          g.moveTo(529,233);
          g.lineTo(596,246);
          g.stroke();
          g.moveTo(530,233);
          g.quadraticCurveTo(528,233,530,234);
          g.stroke();
          g.moveTo(596,246);
          g.quadraticCurveTo(597,246,596,246);
        g.stroke();

        g.beginPath();
          g.moveTo(525,263);
          g.lineTo(587,290);
          g.stroke();
          g.moveTo(526,263);
          g.quadraticCurveTo(524,263,527,264);
          g.stroke();
          g.moveTo(587,290);
          g.quadraticCurveTo(589,291,587,290);
        g.stroke();

        g.beginPath();
          g.moveTo(523,296);
          g.lineTo(581,331);
          g.stroke();
          g.moveTo(524,298);
          g.quadraticCurveTo(522,294,524,297);
          g.stroke();
          g.moveTo(58