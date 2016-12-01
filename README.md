# CSS-Graphica
css的图形库

	<meta name="viewport" content="width=device-width; initial-scale=1.0, minimum-scale=1.0, maximum-scale=1.0, user-scalable=no" />
  在head中引入
  <link rel="stylesheet" type="text/css" href="css/Response.css">//响应式库
  <link rel="stylesheet" type="text/css" href="css/css_library.css">//css图形
<body>
<div class="wrapper">
<div class="ring"></div><!-- 圆环 -->
<div class="Triangle-up"></div><!-- 向上三角形 -->
<div class="Triangle-down"></div><!-- 向下三角形 -->
<div class="Triangle-left"></div><!-- 向左三角形 -->
<div class="Triangle-right"></div><!-- 向右三角形 -->
<div class="Triangle-up-left"></div><!-- 左上三角形 -->
<div class="Triangle-up-right"></div><!-- 右上三角形 -->
<div class="Triangle-down-left"></div><!-- 左下三角形 -->
<div class="Triangle-down-right"></div><!-- 右下三角形 -->
<div class="Arrow-down"></div><!-- 向下箭头 -->
<div class="Trapezoid-like"></div><!-- 等腰梯形 -->
<div class="Parallelogram"></div><!-- 平行四边形 -->
<div class="Hexagon"></div><!-- 六角形 -->
<div class="Five"></div><!-- 五角型 -->
<div class="blank"></div>
<div class="Pentagon"></div><!-- 五边形 -->
<div class="blank"></div>
<div class="Hexagon_b"></div><!-- 六边形 -->
<div class="blank"></div>
<div class="octagon"></div><!-- 八边形 -->
<div class="blank"></div>
<div class="diamond"></div><!-- 菱形 -->
</div>	
</body>

div{margin:0.5rem 0 0 1rem; display: inline-block;}
/*圆环*/
.ring{ width:5rem; height:5rem; border-radius:5rem; border:1px solid #000;}
.ring:after{content: ""; display:block; width:4.5rem; height:4.5rem; border-radius:4.5rem; margin:0.25rem auto;border:1px solid #000; box-sizing:border-box;}
/*向上三角形*/
.Triangle-up{width: 0;height: 0;border-left: 1rem solid transparent;border-right: 1rem solid transparent;border-bottom: 2rem solid #000;}
/*向下三角形*/
.Triangle-down{width: 0;height: 0;border-left: 1rem solid transparent;border-right: 1rem solid transparent;border-top: 2rem solid #000;}
/*向左三角形*/
.Triangle-left{width: 0;height: 0;border-top:1rem solid transparent;border-right: 1rem solid #000;border-bottom: 1rem solid transparent;}
/*向右三角形*/
.Triangle-right{width: 0;height: 0;border-top:1rem solid transparent;border-left: 1rem solid #000;border-bottom:  1rem solid transparent;}
/*左上三角形*/
.Triangle-up-left{width: 0;height: 0;border-top: 1rem solid #000;border-right: 1rem solid transparent}
/*右上三角形*/
.Triangle-up-right{width: 0;height: 0;border-top: 1rem solid #000;border-left: 1rem solid transparent;}
/*左下三角形*/
.Triangle-down-left{width: 0;height: 0;border-bottom: 1rem solid #000;border-right: 1rem solid transparent;}
/*右下三角形*/
.Triangle-down-right{width: 0;height: 0;border-bottom: 1rem solid #000;border-left: 1rem solid transparent;}
/*向下箭头*/
.Arrow-down{position: relative; width: 0; height: 0; border-top: 0.5rem solid transparent; border-right: 0.5rem solid red; -webkit-transform: rotate(10deg); -moz-transform: rotate(10deg);-ms-transform: rotate(10deg); -o-transform: rotate(10deg);}
.Arrow-down:after{content: ""; position: absolute; border: 0 solid transparent; border-top: 0.15rem solid red; border-radius: 1rem 0 0 0; top: -0.6rem; left: -0.45rem; width: 0.6rem; height: 0.6rem; -webkit-transform: rotate(45deg); -moz-transform: rotate(45deg); -ms-transform: rotate(45deg); -o-transform: rotate(45deg);}
/*等腰梯形*/
.Trapezoid-like{border-bottom: 2rem solid red;border-left: 1rem solid transparent;border-right: 1rem solid transparent;height: 0;width: 2rem}
/*平行四边形*/
.Parallelogram{width: 2.25rem;height: 1.5rem;-webkit-transform: skew(20deg); -moz-transform: skew(20deg); -o-transform: skew(20deg);background: red;}
/*六角形*/
.Hexagon{width: 0;height: 0;border-left: 1rem solid transparent;border-right: 1rem solid transparent;border-bottom: 2rem solid red;position: relative;}
.Hexagon:after{width: 0;height: 0;border-left: 1rem solid transparent;border-right:1rem solid transparent;border-top: 2rem solid red;position: absolute;content: "";top:0.6rem;left: -1rem;}
/*五角型*/
.Five{margin: 50px 0; position: relative;display: block; color: red; width: 0px; height: 0px;border-right: 100px solid transparent;border-bottom: 70px solid red;
border-left: 100px solid transparent;-moz-transform: rotate(35deg); -webkit-transform: rotate(35deg);-ms-transform: rotate(35deg);-o-transform: rotate(35deg);}
.Five:before{border-bottom: 80px solid red; border-left: 30px solid transparent; border-right: 30px solid transparent; position: absolute;height: 0; width: 0; top: -45px;left: -65px;display: block; content:""; -webkit-transform: rotate(-35deg); -moz-transform: rotate(-35deg); -ms-transform:rotate(-35deg); -o-transform: rotate(-35deg);}
.Five:after{position: absolute; display: block; color: red; top: 3px;left: -105px;width: 0px;height: 0px;border-right: 100px solid transparent;border-bottom: 70px solid red;border-left: 100px solid transparent;-webkit-transform: rotate(-70deg);-moz-transform: rotate(-70deg); -ms-transform: rotate(-70deg); -o-transform:rotate(-70deg);content:"";}
/*五边形*/
.Pentagon{position: relative; width: 2.7rem; border-width: 2.5rem 0.9rem 0;border-style: solid; border-color: red transparent;}
.Pentagon:after{content: ""; position: absolute; height: 0;width: 0;top: -4.19rem; left: -0.9rem;border-width: 0 2.25rem 1.75rem; border-style: solid; border-color: transparent transparent red;}
/*六边形*/
.Hexagon_b{width: 5.0rem;height: 2.75rem;background: red;position: relative;}
.Hexagon_b:before{content: "";position: absolute;top: -1.25rem;left: 0;width: 0;height: 0;border-left: 2.5rem solid transparent;border-right: 2.5rem solid transparent;border-bottom: 1.253rem solid red;}
.Hexagon_b:after{content: "";position: absolute;bottom: -1.25rem;left: 0;width: 0;height: 0;border-left: 2.5rem solid transparent;border-right: 2.5rem solid transparent;border-top: 1.253rem solid red;}
/*八边形*/
.octagon{width: 4.9rem;height: 5.0rem;background: red;position: relative;}
.octagon:before{content: "";position: absolute;top: 0;left: 0;
border-bottom: 1.45rem solid red;border-left: 1.45rem solid #fff;border-right: 1.45rem solid #fff;width: 2.1rem;height: 0;}
.octagon:after{content: "";position: absolute;bottom: 0;left: 0;border-top: 1.45rem solid red;border-left: 1.45rem solid #fff;border-right: 1.45rem solid #fff;width: 2.1rem;height: 0}
/*菱形*/
.diamond{width: 5.0rem;height: 5.0rem;background: red; transform:rotate(-45deg);}
