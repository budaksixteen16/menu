# menu

<html>
  <head>
    <meta charset="utf-8">
    <title>Menu Responsive</title>
    <link rel="stylesheet" href="css/main_menu_responesive.css">
    <style>
    body {
    margin: 0;
    background: #eff2f7;
    font-family: 'Product Sans';
}
a{
  text-decoration: none;
  color: #353535;
  display: block;
  transition: 0.3s;
}
a:hover {
  transition: 0.3s;
}
nav {
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    background: #fff;
}

.title {
    display: inline-block;
    float: left;
    line-height: 50px;
}

.menu {
    display: inline-block;
    float: right;
}

.menu ul {
    list-style: none;
    padding: 0;
    margin: 0;
}

.menu ul li {
    display: inline-block;
}

.menu ul li a {
    padding: 0 20px;
    display: block;
    line-height: 50px;
}

.menu li:hover{
    background-color: #CDDC39;
}
.wrap{
  width: 80%;
  margin: 0 auto;
}
.tblmenubox {
    display: inline-block;
    float: right;
    line-height: 50px;
}
.tblmenu {
    display: block;
    position: absolute;
    width: 25px;
    height: 25px;
    background: #CDDC39;
    border-radius: 50%;
    top: 50%;
    transform: translateY(-50%);
}
.tblmenubox{
  display: none;
  visibility: hidden;
}
@media screen and (max-width:800px){
  .menu{
    display: none;
  }
  .tblmenubox{
    display: block;
    visibility: visible;
  }
  .menu.sh {
    display: block;
    position: absolute;
    top: 50px;
    background: #CDDC39;
    width: 100%;
    left: 0;
}

.menu a:hover {
    color: #fff;
    background: #353535;
}

.menu ul li {
    display: block;
    text-align: center;
}
}
    </style>
  </head>
  <body>
    <nav>
      <div class="wrap">
      <div class="title">
       Inponow;
      </div>
      <div class="tblmenubox">
        <div class="togel tblmenu">

        </div>
      </div>
      <div class="menu">
        <ul>
          <li><a href="#">Home</a></li>
          <li><a href="#">Contact</a></li>
          <li><a href="#">Service</a></li>
          <li><a href="#">Fiture</a></li>
          <li><a href="#">Maps</a></li>
        </ul>
      </div>
      </div>
    </nav>
    <script src="js/jquery.min.js"></script>
    <script type="text/javascript">
      $(".togel.tblmenu").click(function () {
      $(".menu").toggleClass("sh");
      });
    </script>
  </body>
</html>
