<template>
<div class="fixed-nav sticky-footer bg-dark" id="page-top">
 <nav class="navbar navbar-expand-lg navbar-dark bg-dark fixed-top" id="mainNav">
    
    <div class="collapse navbar-collapse" id="navbarResponsive">
      <div id="logo"><span>项目标题</span></div>
      <ul class="navbar-nav navbar-sidenav" id="exampleAccordion">
        <li class="nav-item" data-toggle="tooltip" data-placement="right" title="Dashboard">
          <a class="nav-link" href="/home">
            <i class="fa fa-fw fa-dashboard"></i>
            <span class="nav-link-text">Dashboard</span>
          </a>
        </li>
        <li class="nav-item" data-toggle="tooltip" data-placement="right" title="Charts">
          <a class="nav-link" href="/home">
            <i class="fa fa-fw fa-area-chart"></i>
            <span class="nav-link-text">Charts</span>
          </a>
        </li>
        <li class="nav-item" data-toggle="tooltip" data-placement="right" title="Tables">
          <a class="nav-link" href="/home">
            <i class="fa fa-fw fa-table"></i>
            <span class="nav-link-text">Tables</span>
          </a>
        </li>
        <li class="nav-item" data-toggle="tooltip" data-placement="right" title="Components">
          <a class="nav-link nav-link-collapse collapsed" data-toggle="collapse" href="#collapseComponents" data-parent="#exampleAccordion">
            <i class="fa fa-fw fa-wrench"></i>
            <span class="nav-link-text">Components</span>
          </a>
          <ul class="sidenav-second-level collapse" id="collapseComponents">
            <li class="nav-second">
              <a href="navbar.html">Navbar</a>
            </li>
            <li class="nav-second">
              <a href="cards.html">Cards</a>
            </li>
          </ul>
        </li>
        <li class="nav-item" data-toggle="tooltip" data-placement="right" title="Example Pages">
          <a class="nav-link nav-link-collapse collapsed" data-toggle="collapse" href="#collapseExamplePages" data-parent="#exampleAccordion">
            <i class="fa fa-fw fa-file"></i>
            <span class="nav-link-text">Example Pages</span>
          </a>
          <ul class="sidenav-second-level collapse" id="collapseExamplePages">
            <li class="nav-second">
              <a href="login.html">Login Page</a>
            </li>
            <li class="nav-second">
              <a href="register.html">Registration Page</a>
            </li>
            <li class="nav-second">
              <a href="forgot-password.html">Forgot Password Page</a>
            </li>
            <li class="nav-second">
              <a href="blank.html">Blank Page</a>
            </li>
          </ul>
        </li>
        <li class="nav-item" data-toggle="tooltip" data-placement="right" title="Link">
          <a class="nav-link" href="#">
            <i class="fa fa-fw fa-link"></i>
            <span class="nav-link-text" >Link</span>
          </a>
        </li>
      </ul>
      <ul class="navbar-nav sidenav-toggler">
        <li class="nav-item">
          <a class="nav-link text-center" id="sidenavToggler">
            <i class=" iconfont fa fa-fw fa-angle-left" v-on:click="test1()" ></i>
          </a>
        </li>
      </ul>
      <ul class="navbar-nav ml-auto">   
        <li class="nav-item">
          <a class="nav-link" data-toggle="modal" data-target="#exampleModal">
            <i class="fa fa-fw fa-sign-out"></i>Logout</a>
        </li>
      </ul>
    </div>
  </nav>
</div>
    
</template>
<script>
export default {
   name :'HomeHeader',
   data(){
      return {}
   } ,
   methods:{
    test1:function(){
        
          $("#sidenavToggler").click(function(e) {
              e.preventDefault();
              $("body").toggleClass("sidenav-toggled");
              $(".navbar-sidenav .nav-link-collapse").addClass("collapsed");
              $(".navbar-sidenav .sidenav-second-level, .navbar-sidenav .sidenav-third-level").removeClass("show");
            });
         },
   }
}
</script>
<style>
@import '../css/sb-admin.css';
@import '../font-awesome-4.7.0/css/font-awesome.css';
        * {
          margin:0;
          padding:0;
          }

        #logo{
        float: left;
        color:#9CD9F9;
        width:320px;
        height:50px;
        line-height: 50px;
        background:url(../images/logo.png);
        background-size:100% 100%;
}

        #logo span{

        margin-left:20%;
        font-size: 20px;
          
        }
 
</style>


