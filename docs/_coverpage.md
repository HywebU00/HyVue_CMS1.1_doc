<!-- _coverpage.md -->
<!-- # HyUI <small>4.0</small> -->

<div class="info">

<h1>
<span class="title"><img src="cover_logo_w.png"  style="max-width:350px;"></span>
<span class="admin">Admin Dashboard</span>
</h1>

<div class="subtitle">
<p>透過 Vuetify3 文件搭建的ＵＩ模版，快速搭建後台頁面</p>
</div>

<div class="btnList">
<span >
  <a href="#?id=hyvue-cms">Get Started</a>
</span>
<span >
  <a class="github" href="https://github.com/HywebU00/HyVue_CMS1.1">GitHub</a>
</span>
</div>
</div>

<style>
  .logo{
    width: 360px;
    margin: 0 auto;
    position: relative;
  }
  .logo span{
    margin-right: 2em;
    text-align: end;
    position: absolute;
    top: 1.25em;
    color:#336699;
    right: 0;
  }
  
  section.cover a{
    border-radius: 0.5rem;
    color:#fff;
    display: inline-block;
    font-size: 1.05rem;
    letter-spacing: .1rem;
    margin: 0.5rem 1rem;
    padding: 0.75em 2rem;
    text-decoration: none;
    transition: all .15s ease;
    width:180px;
    margin: 0.25em;
    background: #fff;
    color:#044d7f;
background-size: 300% 100%;
}
section.cover a:hover{
background-position: 100% 0;
moz-transition: all .4s ease-in-out;
-o-transition: all .4s ease-in-out;
-webkit-transition: all .4s ease-in-out;
transition: all .4s ease-in-out;
background: #057BB7;
color:#fff;
}
section.cover a.github{
border:1px solid #fff !important;
background:unset;
color:#fff;
transition: all .4s ease-in-out;


}
section.cover a.github:hover{
  background:#057BB7;
  border:1px solid #057BB7!important;
  color:#fff;

}

.subtitle{
  margin-top:2rem;
 
}

.cover.show{
background-image: url(cover_bg.jpg) !important;
background-repeat: no-repeat !important;
background-position: center !important;

}

.cover.show:after{
background-position: center;
}
.info{
margin: 0 0 10% 0;
}

.cover.show:after{
content:'';
background-image: url(cover_bg.png) !important;

width: 100%;
position: absolute;
height: 100%;
z-index: -1;
    background-repeat: no-repeat;
    background-size: cover;
    background-position: right;

}
section.cover h1{
color:#fff;
font-size: 3rem;
font-weight: 700;
margin:0.75em 0 0 0;

}
section.cover h1 .admin{
margin-top:-0.5rem;
display: block;
font-weight: 500;
font-size: 2.3rem;
font-family:sans-serif;
letter-spacing: -0.1rem;
}
section.cover p {
font-size: 1.2em;
color:#fff;
margin-top: 3em;
margin-bottom:1.75em;
}
.app-nav li {
  color:#fff;
}
.app-nav li ul li{
  color:#333;
}
</style>
