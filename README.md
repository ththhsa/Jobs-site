<!doctype html>
<html lang="en">

<head>
  <!-- Required meta tags -->
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">

  <!-- Bootstrap CSS -->
  <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css" >
  <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0-beta.2/css/bootstrap.min.css" >
  <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/font-awesome/4.7.0/css/font-awesome.min.css">
  <link href="https://fonts.googleapis.com/css2?family=Oswald&display=swap" rel="stylesheet">

  <link rel="stylesheet" href="styles.css">
<style>
  * {
  margin: 0;
  padding: 0;   
  box-sizing: border-box;
      
}

body,
html {
  height: 100%;
}

header {
  /* background: #2d2d7f !important; */
  background-image: url("https://images.unsplash.com/photo-1541746972996-4e0b0f43e02a?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=500&q=60");
  background-repeat: no-repeat;
  background-attachment: fixed;
  background-size: 100% 100%;
}

/* main-header start */

[data-target="#mainMenu"] {
  position: relative;
  z-index: 999;
}

#mainMenu li > a {
  font-size: 16px;
  letter-spacing: 1px;
  color: #fff;
  font-weight: 400;
  /* position relative to its previous postion */
  position: relative;
  z-index: 1;
  text-decoration: none;
}

.main-header.fixed-nav #mainMenu li > a {
  color: #fff;
  text-decoration: none;
}

#mainMenu li:not(:last-of-type) {
  margin-right: 30px;
}

#mainMenu li > a::before {
  position: absolute;
  content: "";
  width: calc(100% - 1px);
  height: 1px;
  background: #fff;
  bottom: -6px;
  left: 0;
  -webkit-transform: scale(0, 1);
  -ms-transform: scale(0, 1);
  transform: scale(0, 1);
  -webkit-transform-origin: right center;
  -ms-transform-origin: right center;
  transform-origin: right center;
  z-index: -1;
  -webkit-transition: transform 0.5s ease;
  transition: transform 0.5s ease;
}

#mainMenu li > a:hover::before,
#mainMenu li > a.active::before {
  -webkit-transform: scale(1, 1);
  -ms-transform: scale(1, 1);
  transform: scale(1, 1);
  -webkit-transform-origin: left center;
  -ms-transform-origin: left center;
  transform-origin: left center;
}

.main-header.fixed-nav #mainMenu li > a::before {
  background: #000;
}

.main-header {
  position: relative;
  left: 0;
  z-index: 99;
  width: 100%;
  -webkit-transition: all 0.4s ease;
  transition: all 0.4s ease;
}

.main-header.fixed-nav {
  top: 0;
  background: #fff;
  -webkit-box-shadow: 0 8px 12px -8px rgba(0, 0, 0, 0.09);
  box-shadow: 0 8px 12px -8px rgba(0, 0, 0, 0.09);
  -webkit-transition: all 0.4s ease;
  transition: all 0.4s ease;
}

/* main-header end */

@media (max-width: 991px) {
  /*header starts*/

  .collapse.in {
    display: block !important;
    padding: 0;
    clear: both;
  }
  .navbar-toggler {
    margin: 0;
    padding: 0;
    width: 40px;
    height: 40px;
    position: absolute;
    top: 25px;
    right: 0;
    border: none;
    border-radius: 0;
    outline: none !important;
  }
  .main-header .navbar {
    float: none;
    width: 100%;
    padding-left: 0;
    padding-right: 0;
    text-align: center;
  }
  .main-header .navbar-nav {
    margin-top: 70px;
  }
  .main-header .navbar-nav li .nav-link {
    text-align: center;
    padding: 20px 15px;
    border-radius: 0px;
  }
  /**/
  .main-header .navbar-toggler .icon-bar {
    background-color: #fff;
    margin: 0 auto 6px;
    border-radius: 0;
    width: 30px;
    height: 3px;
    position: absolute;
    right: 0;
    -webkit-transition: all 0.2s ease;
    transition: all 0.2s ease;
  }
  .main-header .navbar .navbar-toggler .icon-bar:first-child {
    margin-top: 3px;
  }
  .main-header .navbar-toggler .icon-bar-1 {
    width: 10px;
    top: 0px;
  }
  .main-header .navbar-toggler .icon-bar-2 {
    width: 16px;
    top: 12px;
  }
  .main-header .navbar-toggler .icon-bar-3 {
    width: 20px;
    top: 21px;
  }
  .main-header .current .icon-bar {
    margin-bottom: 5px;
    border-radius: 0;
    display: block;
  }
  .main-header .current .icon-bar-1 {
    width: 18px;
  }
  .main-header .current .icon-bar-2 {
    width: 30px;
  }
  .main-header .current .icon-bar-3 {
    width: 10px;
  }
  .main-header .navbar-toggler:hover .icon-bar {
    background-color: #fff;
  }
  .main-header .navbar-toggler:focus .icon-bar {
    background-color: #fff;
  }
  /*header ends*/
  #mainMenu li {
    width: 120px;
    text-align: left;
    margin-left: 30%;
    margin-bottom: 10px;
  }

  .banner {
    padding-top: 150px;
  }
  .dropdown-toggle{
    padding-right: 55px;
  }
  .dropdown-content{
    margin-left: 47%;
  }
}

/* Dropdown Content (Hidden by Default) */

.dropdown-content {
  display: none;
  position: absolute;
  /* background-color: #f1f1f1; */
  min-width: fit-content;
  box-shadow: 0px 8px 16px 0px rgba(0, 0, 0, 0.2);
  z-index: 1;
}

/* Links inside the dropdown */

.dropdown-content a {
  color: black;
  padding: 12px 16px;
  text-decoration: none;
  display: block;
}

/* Change color of dropdown links on hover */

.dropdown-content a:hover {
  background-color: #ddd;
}

/* Show the dropdown menu on hover */

.dropdown:hover .dropdown-content {
  display: block;
}

/* section starts */

.banner {
  height: 80vh;
  background-image: url("https://images.unsplash.com/photo-1541746972996-4e0b0f43e02a?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=500&q=60");
  background-position: center;
  background-size: cover;
  color: #fff;
}

.banner h1 {
  font-size: 50px;
  font-weight: 600;
  text-shadow: 0 0 30px rgba(0, 0, 0, 0.5);
}

.banner p {
  padding-top: 15px;
  line-height: 150%;
  font-size: larger;
  text-shadow: 0 0 30px rgba(0, 0, 0, 0.5);
}
@media (max-width: 321px){
.banner p{
  display: none;
}
.search-job {
  margin-top:-20px;
}
}
/* search bar */

.search-job {
  padding: 30px 0;
  margin: -50px 6% 50px;
  background-image: linear-gradient(to right, #b3b3b3, #57606f);
}
@media (max-width: 514px){
.search-job {
  margin-top:-15px;
}
}
.search-job .form-control {
  max-width: 250px;
  display: inline-flex;
  margin: 10px 5px;
  height: 50px;
  border-radius: 25px;
  box-shadow: none !important;
  border: none !important;
  padding-left: 30px;
}

.search-job .btn-primary {
  width: 150px;
  border-radius: 25px;
  box-shadow: none !important;
  border: none;
  height: 50px;
  margin: 5px;
  padding: 5px 20px;
  display: table-cell;
  vertical-align: middle;
}

.search-job .btn-primary:hover {
  border: 1px solid yellow;
}

/* top recuruiters */

#recruiters {
  padding-top: 50px;
  padding-bottom: 100px;
}

#recruiters h3 {
  text-align: center;
  padding-bottom: 40px;
}

h3::before {
  content: "";
  background-image: linear-gradient(to right, #6db9ef, #7ce08a);
  width: 50px;
  height: 30px;
  position: absolute;
  z-index: -10;
  margin-top: -15px;
  border-top-left-radius: 70px;
  border-bottom-right-radius: 90px;
}

#recruiters img {
  max-width: 100px;
  margin: 10px 20px;
}

.col-md-3 {
  display: inline-block;
  margin-left: -4px;
}

.col-md-3 img {
  width: 100%;
  height: auto;
}

body .carousel-indicators li {
  background-color: red;
}

body .carousel-control-prev-icon,
body .carousel-control-next-icon {
  background-color: red;
}

body .no-padding {
  padding-left: 0;
  padding-right: 0;
}

/* category wise jobs */

.category ul li {
  list-style: none;
}

.category {
  padding: 30px;
  border-radius: 10px;
  margin: 20px 0;
  box-shadow: 0 2px 40px 0 rgba(110, 130, 208, 0.18);
}

.jobcategory {
  width: 20%;
}

.categories {
  display: inline-flex;
  justify-content: space-evenly;
}

h5 {
  border-bottom: 1px solid black;
}

@media only screen and (max-width: 1000px) {
  .categories {
    display: flex;
    flex-direction: column;
    justify-content: center;
  }
  .jobcategory {
    width: 80%;
    margin-left: auto;
    margin-right: auto;
  }
}

/* recent jobs */

#jobs {
  background: #f8f8fa;
  padding: 50px 0;
}

.company-details {
  box-shadow: 0 2px 70px 0 rgba(110, 130, 208, 0.18);
  border-radius: 5px;
  margin-bottom: 20px;
}

.job-update {
  background: white;
  padding: 10px 20px;
  border-radius: 5px;
}

.job-update h4 strong {
  font-size: 30px;
  font-family: "Oswald", sans-serif;
}

.job-update .fa {
  margin-top: 5px;
  margin-right: 10px;
  color: #77d1b1;
}

.price {
  color: #018f62;
}

.location {
  color: red;
}

/* .description {
  display: none;
}
.company-details :hover .description {
  display: block;
}
 */


.description {
    overflow: hidden; 
    height: 0; opacity: 0;
    transition: height 0ms 400ms, opacity 400ms 0ms;
}
.company-details :hover .description{
    height: auto; opacity: 1;
    transition: height 0ms 0ms, opacity 600ms 0ms;
}


.bookmark{
  color: #000 !important;
  float: right;
  display: inline-flex;
  font-size: 20px;
  cursor: pointer;
}

.bookmark p{
  margin-left: 5px;
    font-size: 20px;
    cursor: pointer;

}
.fa-heart-o:before {
    content: "\f08a";
    margin-right: 8px;
      font-size: 20px;
      cursor: pointer;
      
    color: rgb(33, 33, 226) !important;

}
.fa-heart-o:before .bookmark{
  color: rgb(33, 33, 226) !important;
}
.fa-heart:before {
    content: "\f004";
    margin-right: 8px;
      font-size: 20px;
      cursor: pointer;
      color: rgb(33, 33, 226) !important;
}




.job-update small {
  background: #efefef;
  padding: 1px 5px;
  margin: 0 5px;
}

.job-update small:hover {
  cursor: pointer;
  background: #23c0e9;
  z-index: 2;
  transition: all 200ms ease-in;
  transform: scale(1.1);
  color: white;
}

.job-update p {
  margin-bottom: 0 !important;
}

.job-update a {
  text-decoration: none !important;
  color: #b6bed2;
  float: right;
}

.job-update a:hover {
  text-decoration: none !important;
  color: rgb(0, 95, 238);
  float: right;
}

.apply-btn {
  height: 40px;
  background-image: linear-gradient(to right, #6db9ef, #111136);
  padding: 5px;
  border-bottom-left-radius: 5px;
}

.apply-btn .btn-primary {
  padding: 0 30px;
  float: right;
  box-shadow: none !important;
  background: transparent;
  border: 1px solid #fff;
  width: 100px;
  height: 30px;
  line-height: 30px;
  background: #f36969;
  color: #ffffff;
  font-size: 16px;
  text-transform: uppercase;
  border-radius: 10px;
}

.pagelink li {
  height: 25px;
  list-style: none;
  width: 25px;
  display: inline-block;
  cursor: pointer;
}

.pagelink li:hover,
.activa {
  color: #fff;
  background-image: linear-gradient(to right, #6db9ef, #7ce08a);
}

.left-arrow {
  color: #999;
}

.right-arrow {
  color: #29b929;
}

/* site-stats */

#site-stats {
  padding: 100px 0;
}

#site-stats {
  margin-bottom: 30px;
}

.stats-box {
  padding: 30px;
  border-radius: 10px;
  margin: 20px 0;
  box-shadow: 0 2px 40px 0 rgba(110, 130, 208, 0.18);
}

.stats-box:hover {
  transition: all 0.2s ease-out;
  box-shadow: 0px 4px 8px rgba(38, 38, 38, 0.2);
  border: 1px solid #cccccc;
  background-color: #00838d;
  transform: scale(1.1);
}

.stats-box:hover p {
  transition: all 0.3s ease-out;
  color: #ffffff;
}

.stats-box:hover i {
  transition: all 0.3s ease-out;
  color: #ffffff;
}

.stats-box:hover small {
  transition: all 0.3s ease-out;
  color: #ffffff;
}

.stats-box .fa {
  font-size: 30px;
  margin-right: 10px;
  margin-bottom: 10px;
}

/* footer */

.page-footer {
  background-color: rgb(37, 28, 28);
}

.icon_name {
  padding-left: 10px;
  cursor: pointer;
}

.icon_name:hover {
  color: #00ff00;
}

.dark-grey-text {
  color: #fff;
}
  </style>
  <title>Job Portal Landing Page</title>
</head>

<body>

  <!-- header starts -->
  <header class="main-header">
    <div class="container">
      <nav class="navbar navbar-expand-lg main-nav px-0">
        <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#mainMenu"
          aria-controls="mainMenu" aria-expanded="false" aria-label="Toggle navigation">
          <span class="icon-bar icon-bar-1"></span>
          <span class="icon-bar icon-bar-2"></span>
          <span class="icon-bar icon-bar-3"></span>
        </button>
        <div class="collapse navbar-collapse" id="mainMenu">
          <ul class="navbar-nav ml-auto text-uppercase f1">
            <li>
              <a href="https://www.youtube.com/@ShamodFirezz" class=" active-first">Home</a>
            </li>
            <li>
              <a href="https://www.youtube.com/@ShamodFirezz">About us</a>
            </li>
            <li>
              <a href="https://www.youtube.com/@ShamodFirezz">All Jobs</a>
            </li>
            <li>
              <a href="https://www.youtube.com/@ShamodFirezz">Interships</a>
            </li>
            <li>
              <a href="https://www.youtube.com/@ShamodFirezz">Govt. Jobs</a>
            </li>
            <li>
              <a href="https://www.youtube.com/@ShamodFirezz">Contact us</a>
            </li>
          </ul>
          <div class="nav-item dropdown ml-auto">
            <a class="dropdown-toggle dropbtn" href="#" id="navbarDropdownMenuLink" role="button" data-toggle="dropdown"
              aria-haspopup="true" aria-expanded="false">
              <img src="https://s3.eu-central-1.amazonaws.com/bootstrapbaymisc/blog/24_days_bootstrap/fox.jpg"
                width="40" height="40" class="rounded-circle">
            </a>
            <div class="dropdown-menu dropdown-content" aria-labelledby="navbarDropdownMenuLink">
              <a class="dropdown-item" href="#">Dashboard</a>
              <a class="dropdown-item" href="#">Edit Profile</a>
              <a class="dropdown-item" href="#">Log Out</a>
            </div>
          </div>

        </div>
      </nav>
    </div>
    <!-- /.container -->
  </header>

  <!-- header ends -->

  <!-- section 2 -->
  <div class="banner text-center">
    <h1><span style="color: aqua; font-size: 1.7em;">JoblyHub</span> Jobs in Europe & America</h1>
    <p>Find your dream job faster! Discover the best remote, freelance, and full-time opportunities in one place</p>
  </div>

  <!-- search box -->
  <div class="search-job text-center">
    <input type="text" class="form-control" placeholder="Skills, Job Title, Designation">
    <input type="text" class="form-control" placeholder="Location">
    <input type="text" class="form-control" placeholder="Experience">
   <a href="https://cineverse85.netlify.app/" target="new window"> <input type="button" class="btn btn-primary" value="Search"></a>
  </div>


  <!-- top recuriters -->
  <section id="recruiters">
    <div class="container text-center">
      <h3>TOP RECRUITERS</h3>
      <div>
        <img
          src="https://i.gadgets360cdn.com/large/oracle_reuters_full_1570520864400.JPG?output-quality=80&output-format=webp"
          alt="">
        <img
          src="https://img.etimg.com/thumb/msid-65905312,width-300,imgsize-269627,,resizemode-4,quality-100/zomato.jpg"
          alt="">
        <img src="https://www.oneindia.com/img/2017/07/swiggy-19-1500443913.jpg" alt="">
        <img
          src="https://prnewswire2-a.akamaihd.net/p/1893751/sp/189375100/thumbnail/entry_id/1_rkna5p3b/def_height/67/def_width/200/version/100031/type/1"
          alt="">
        <img src="https://upload.wikimedia.org/wikipedia/en/thumb/3/3d/Wipro_logo.svg/1200px-Wipro_logo.svg.png" alt="">
        <img src="https://ciotechie.com/wp-content/uploads/2019/04/4_1-3.png" alt="">
      </div>
      <div>
        <img
          src="https://prnewswire2-a.akamaihd.net/p/1893751/sp/189375100/thumbnail/entry_id/1_rkna5p3b/def_height/67/def_width/200/version/100031/type/1"
          alt="">
        <img src="https://upload.wikimedia.org/wikipedia/en/thumb/3/3d/Wipro_logo.svg/1200px-Wipro_logo.svg.png" alt="">
        <img src="https://ciotechie.com/wp-content/uploads/2019/04/4_1-3.png" alt="">
        <img
          src="https://i.gadgets360cdn.com/large/oracle_reuters_full_1570520864400.JPG?output-quality=80&output-format=webp"
          alt="">
        <img
          src="https://img.etimg.com/thumb/msid-65905312,width-300,imgsize-269627,,resizemode-4,quality-100/zomato.jpg"
          alt="">
        <img src="https://www.oneindia.com/img/2017/07/swiggy-19-1500443913.jpg" alt="">

      </div>
      <div>
        <img
          src="https://i.gadgets360cdn.com/large/oracle_reuters_full_1570520864400.JPG?output-quality=80&output-format=webp"
          alt="">
        <img
          src="https://img.etimg.com/thumb/msid-65905312,width-300,imgsize-269627,,resizemode-4,quality-100/zomato.jpg"
          alt="">
        <img src="https://upload.wikimedia.org/wikipedia/en/thumb/3/3d/Wipro_logo.svg/1200px-Wipro_logo.svg.png" alt="">
        <img src="https://ciotechie.com/wp-content/uploads/2019/04/4_1-3.png" alt="">
        <img src="https://www.oneindia.com/img/2017/07/swiggy-19-1500443913.jpg" alt="">
        <img
          src="https://prnewswire2-a.akamaihd.net/p/1893751/sp/189375100/thumbnail/entry_id/1_rkna5p3b/def_height/67/def_width/200/version/100031/type/1"
          alt="">

      </div>
    </div>
  </section>

  <!-- category wise search -->

  <section class="category">
    <div class="container text-left">
      <h3 class="text-center">Jobs by category</h3>
      <div class="row">

        <div class="col-md-12 categories">

          <div class="jobcategory category">
            <h5 class="side-title">Jobs by Skills</h5>
            <ul>
              <li><a href="https://poawooptugroo.com/4/8888971" target="newwindow" title="">Business <span class="pull-right">13</span></a></li>
              <li><a href="https://poawooptugroo.com/4/8888971" title="">Technology <span class="pull-right">13</span></a></li>
              <li><a href="https://poawooptugroo.com/4/8888971" title="">Web <span class="pull-right">13</span></a></li>
              <li><a href="https://poawooptugroo.com/4/8888971" title="">Ecommerce <span class="pull-right">13</span></a></li>
              <li><a href="https://poawooptugroo.com/4/8888971" title="">Wordpress <span class="pull-right">13</span></a></li>
              <li><a href="https://poawooptugroo.com/4/8888971" title="">Data analysis <span class="pull-right">13</span></a></li>
              <li><a href="https://poawooptugroo.com/4/8888971" title="">Digital marketing <span class="pull-right">13</span></a></li>
              <li><a href="https://poawooptugroo.com/4/8888971" title="">Machine Learning <span class="pull-right">13</span></a></li>
            <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>More Button with Link</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin: 50px;
        }

        .more-btn {
            background-color: #007bff;
            color: white;
            padding: 10px 20px;
            font-size: 18px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            text-decoration: none;
            display: inline-block;
            transition: 0.3s;
        }

        .more-btn:hover {
            background-color: #0056b3;
        }
    </style>
</head>
<body>

    <p></p>

    <!-- "More" button with a link -->
    <a href="https://cineverse85.netlify.app/" class="more-btn" target="_blank">More</a>

</body>
</html>
  
            </ul>
           
          </div>
          
          <div class="jobcategory category">
            <h5 class="side-title">Jobs Types</h5>
            <ul>
              <li><a href="https://www.youtube.com/@ShamodFirezz" title="">Freshers Job <span class="pull-right">13</span></a></li>
              <li><a href="https://www.youtube.com/@ShamodFirezz" title="">Freelancing <span class="pull-right">13</span></a></li>
              <li><a href="https://www.youtube.com/@ShamodFirezz" title="">Unpaid Internships <span class="pull-right">13</span></a></li>
              <li><a href="https://www.youtube.com/@ShamodFirezz" title="">Paid Internships <span class="pull-right">13</span></a></li>
              <li><a href="https://www.youtube.com/@ShamodFirezz" title="">Walk-In Jobs <span class="pull-right">13</span></a></li>
              <li><a href="https://www.youtube.com/@ShamodFirezz" title="">Part-Time Jobs <span class="pull-right">13</span></a></li>
              <li><a href="https://www.youtube.com/@ShamodFirezz" title="">Full-Time Jobs <span class="pull-right">13</span></a></li>
              <li><a href="https://www.youtube.com/@ShamodFirezz" title="">Wrok From Home <span class="pull-right">13</span></a></li>
             <!-- "More" button with a link -->
    <a href="https://cineverse85.netlify.app/" class="more-btn" target="_blank">More</a>

</body>
</html> 
            </ul>
         
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- recent jobs -->
  <section id="jobs">
    <div class="container">
      <h5>RECENT JOB UPDATES</h5>

      <div class="company-details">
        <div class="job-update">
          <h4><strong> Frontend Developer </strong>
          <i class="fa fa-heart-o bookmark"><p>
            Save Job</p></i></h4>
          <h6></h6>
          <i class="fa fa-briefcase"></i><span>0-1 years</span><br>
          <i class="fa fa-inr"></i><span class="price"> 50000 to 70000 </span><br>
          <i class="fa fa-map-marker"></i><span class="location"> Lahore</span>
          <p><strong>Skills</strong> <i class="fa fa-angle-double-right"></i><small> Java</small><small> Web
              scrapping</small><small>
              Django</small><small> Flask</small></p>
          <p class="description"><strong>Description</strong> <i class="fa fa-angle-double-right"></i>
            Shaheen Developers is seeking a talented and experienced Frontend Developer to join our forward-thinking team. We are committed to innovation and delivering exceptional digital experiences. If you're passionate about creating intuitive user interfaces, working with cutting-edge technologies, and contributing to impactful projects, we’d love to hear from you.<a href="https://www.youtube.com/@ShamodFirezz"> Read More</a></p>
        </div>
        <div class="apply-btn">
          <button type="button" class="btn btn-primary" a href="https://www.youtube.com/@ShamodFirezz">target="_blank">Apply</button></a> 
        </div>
      </div>
      <div class="company-details">
        <div class="job-update">
          <h4><strong>Frontend Web Developer - Mid Level </strong>
            <i class="fa fa-heart-o bookmark">
              <p>
                Save Job</p>
            </i></h4>
          <h6></h6>
          <i class="fa fa-briefcase"></i><span>0-1 years</span><br>
          <i class="fa fa-inr"></i><span class="price"> 95000 to 100000</span><br>
          <i class="fa fa-map-marker"></i><span class="location"> Islamabad</span>
          <p><strong>Skills</strong> <i class="fa fa-angle-double-right"></i><small> Java</small><small> Web
              scrapping</small><small>
              Django</small><small> Flask</small></p>
          <p class="description"><strong>Description</strong> <i class="fa fa-angle-double-right"></i>
            We are looking for a highly skilled and motivated Frontend Developer to join our team. The ideal candidate will have expertise in building visually stunning and user-friendly interfaces, translating Figma designs into pixel-perfect HTML/CSS, and a strong command of JavaScript.. <a href="#"> Read More</a></p>
        </div>
        <div class="apply-btn">
          <a class="dark-grey-text" href="https://www.youtube.com/@ShamodFirezz"><button type="button" class="btn btn-primary" target="_blank">Apply</button></a>
        </div>
      </div>
      <div class="company-details">
        <div class="job-update">
          <h4><strong> Senior Python Devloper </strong>
            <i class="fa fa-heart-o bookmark">
              <p>
                Save Job</p>
            </i></h4>
          <h6></h6>
          <i class="fa fa-briefcase"></i><span>0-1 years</span><br>
          <i class="fa fa-inr"></i><span class="price"> 100000 to 150k</span><br>
          <i class="fa fa-map-marker"></i><span class="location"> Lahore</span>
          <p><strong>Skills</strong> <i class="fa fa-angle-double-right"></i><small> Java</small><small> Web
              scrapping</small><small>
              Django</small><small> Flask</small></p>
          <p class="description"><strong>Description</strong> <i class="fa fa-angle-double-right"></i>
            Works independently under limited supervision and applies knowledge of subject matter in Applications
            Development. Possess sufficient knowledge and skills to effectively deal with issues, challenges within
            field of specialization to develop simple applications solutions.
            Second level professional with direct impact on
            results and outcome. <a href="#"> Read More</a></p>
        </div>
        <div class="apply-btn">
          <a class="dark-grey-text" href="https://www.youtube.com/@ShamodFirezz"><button type="button" class="btn btn-primary" target="_blank">Apply</button></a>
        </div>
      </div>
      <div class="company-details">
        <div class="job-update">
                    <h4><strong> Dot Net Developer </strong>
                      <i class="fa fa-heart-o bookmark">
                        <p>
                          Save Job</p>
                      </i></h4>
          <h6>XYZ private limited</h6>
          <i class="fa fa-briefcase"></i><span>0-1 years</span><br>
          <i class="fa fa-inr"></i><span class="price"> 55000 to 65000</span><br>
          <i class="fa fa-map-marker"></i><span class="location"> Karachi</span>
          <p><strong>Skills</strong> <i class="fa fa-angle-double-right"></i><small> Java</small><small> Web
              scrapping</small><small>
              Django</small><small> Flask</small></p>
          <p class="description"><strong>Description</strong> <i class="fa fa-angle-double-right"></i>
            We are delighted to be offering this unique opportunity for a talented .NET Software Developer to join our growing friendly team. We are looking for someone with commercial experience as a .NET Software Developer to join us and be responsible for developing and supporting in house insurance application as well as analyse, develop, and test all applications using the appropriate processes, methods, and standards. <a href="#"> Read More</a></p>
        </div>
        <div class="apply-btn">
         <a class="dark-grey-text" href="https://www.youtube.com/@ShamodFirezz"><button type="button" class="btn btn-primary" target="_blank">Apply</button></a>
        </div>
      </div>
      <div class="company-details">
        <div class="job-update">
                    <h4><strong> Web Application Developer </strong>
                      <i class="fa fa-heart-o bookmark">
                        <p>
                          Save Job</p>
                      </i></h4>
          <h6>XYZ private limited</h6>
          <i class="fa fa-briefcase"></i><span>0-1 years</span><br>
          <i class="fa fa-inr"></i><span class="price">100k - 150k</span><br>
          <i class="fa fa-map-marker"></i><span class="location"> Lahore</span>
          <p><strong>Skills</strong> <i class="fa fa-angle-double-right"></i><small> Java</small><small> Web
              scrapping</small><small>
              Django</small><small> Flask</small></p>
          <p class="description"><strong>Description</strong> <i class="fa fa-angle-double-right"></i>
            We at hashlogics seeking sharp-minded and talented graduates to join our team as Junior Bubble.io Developers. In this role, you will undergo comprehensive training in the Bubble.io platform and gain hands-on experience in developing robust web applications. This is an excellent opportunity for recent graduates with a passion for problem-solving, data structures and algorithms, and database management to kick-start their career in software development.. <a href="#"> Read More</a></p>
        </div>
        <div class="apply-btn">
          <a class="dark-grey-text" href="https://www.youtube.com/@ShamodFirezz"><button type="button" class="btn btn-primary" target="_blank">Apply</button></a>
        </div>
      </div>
      <div class="company-details">
        <div class="job-update">
                    <h4><strong> Urgently Hiring React JS Developer </strong>
                      <i class="fa fa-heart-o bookmark">
                        <p>
                          Save Job</p>
                      </i></h4>
          <h6></h6>
          <i class="fa fa-briefcase"></i><span>0-1 years</span><br>
          <i class="fa fa-inr"></i><span class="price"> 4.00 - 5.00 Lacs P.A</span><br>
          <i class="fa fa-map-marker"></i><span class="location"> Gujrat</span>
          <p><strong>Skills</strong> <i class="fa fa-angle-double-right"></i><small> Java</small><small> Web
              scrapping</small><small>
              Django</small><small> Flask</small></p>
          <p class="description"><strong>Description</strong> <i class="fa fa-angle-double-right"></i>
            Preesoft Pvt Ltd is seeking a skilled React.js Developer with 2-3 years of experience to join our growing team. The ideal candidate should have a strong understanding of JavaScript, solid experience with React.js, and the ability to collaborate effectively in a fast-paced environment. This role will involve building and enhancing user-facing features, ensuring high performance, and delivering a seamless user experience.

 <a href="https://www.youtube.com/@ShamodFirezz"> Read More</a></p>
        </div>
        <div class="apply-btn">
          <button type="button" class="btn btn-primary" target="_blank">Apply</button>
        </div>
      </div>
      <ul class="pagelink text-center">
        <li class="right-arrow">&#8592;</li>
        <li class="active">1</li>
        <li>2</li>
        <li>3</li>
        <li>4</li>
        <li class="right-arrow">&#8594;</li>
      </ul>
    </div>
  </section>







  <!-- site stats -->
  <section id="site-stats">
    <div class="container text-center">
      <h3>JOBSITE STATS</h3>
      <div class="row">
        <div class="col-md-6">
          <div class="row">
            <div class="col-md-6">
              <div class="stats-box">
                <i class="fa fa-user-o"></i><span><small>100k + </small></span>
                <p>Job Seekers</p>
              </div>
            </div>
            <div class="col-md-6">
              <div class="stats-box">
                <i class="fa fa-slideshare"></i><span><small>500k + </small></span>
                <p>Recruiters</p>
              </div>
            </div>
          </div>
        </div>
        <div class="col-md-6">
          <div class="row">
            <div class="col-md-6">
              <div class="stats-box">
                <i class="fa fa-hand-peace-o"></i><span><small>10k + </small></span>
                <p>Active Jobs</p>
              </div>
            </div>
            <div class="col-md-6">
              <div class="stats-box">
                <i class="fa fa-building"></i><span><small>400k + </small></span>
                <p>Companies</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
  <!-- Footer -->
  <footer class="page-footer font-small blue-grey lighten-5">

    <!-- Footer Links -->
    <div class="container text-center text-md-left mt-3 pt-5">

      <!-- Grid row -->
      <div class="row mt-3 dark-grey-text">

        <!-- Grid column -->
        <div class="col-md-3 col-lg-4 col-xl-3 mb-4">



          <!-- Links -->
          <h6 class="text-uppercase font-weight-bold text-light">Information</h6>
          <hr class="teal accent-3 mb-4 mt-0 d-inline-block mx-auto" style="width: 60px;">
          <p>
            <a class="dark-grey-text" href="https://www.youtube.com/@ShamodFirezz">About Us</a>
          </p>
          <p>
            <a class="dark-grey-text" href="https://www.youtube.com/@ShamodFirezz">Contact Us</a>
          </p>
          <p>
            <a class="dark-grey-text" href="https://www.youtube.com/@ShamodFirezz">Terms Of Use</a>
          </p>
          <p>
            <a class="dark-grey-text" href="https://www.youtube.com/@ShamodFirezz">FAQs</a>
          </p>

        </div>
        <!-- Grid column -->

        <!-- Grid column -->
        <div class="col-md-2 col-lg-2 col-xl-2 mx-auto mb-4">

          <!-- Links -->
          <h6 class="text-uppercase font-weight-bold text-light">Job seekers</h6>
          <hr class="teal accent-3 mb-4 mt-0 d-inline-block mx-auto" style="width: 60px;">
          <p>
            <a class="dark-grey-text" href="https://www.youtube.com/@ShamodFirezz">Job Search</a>
          </p>
          <p>
            <a class="dark-grey-text" href="https://www.youtube.com/@ShamodFirezz">Career Advices</a>
          </p>
          <p>
            <a class="dark-grey-text" href="https://www.youtube.com/@ShamodFirezz">Resume Builder</a>
          </p>
          <p>
            <a class="dark-grey-text" href="https://www.youtube.com/@ShamodFirezz">Report a Problem</a>
          </p>

        </div>
        <!-- Grid column -->

        <!-- Grid column -->
        <div class="col-md-3 col-lg-2 col-xl-2 mx-auto mb-4">

          <!-- Links -->
          <h6 class="text-uppercase font-weight-bold text-light">Employers</h6>
          <hr class="teal accent-3 mb-4 mt-0 d-inline-block mx-auto" style="width: 60px;">
          <p>
            <a class="dark-grey-text" href="https://www.youtube.com/@ShamodFirezz">Job Posting</a>
          </p>
          <p>
            <a class="dark-grey-text" href="https://www.youtube.com/@ShamodFirezz">Advertise With Us</a>
          </p>
          <p>
            <a class="dark-grey-text" href="https://www.youtube.com/@ShamodFirezz">Access Resumes</a>
          </p>
          <p>
            <a class="dark-grey-text" href="https://www.youtube.com/@ShamodFirezz">FAQs</a>
          </p>

        </div>
        <!-- Grid column -->

        <!-- Grid column -->
        <div class="col-md-4 col-lg-3 col-xl-3 mx-auto mb-md-0 mb-4">

          <!-- Links -->
          <h6 class="text-uppercase font-weight-bold text-light">Stay Connected</h6>
          <hr class="teal accent-3 mb-4 mt-0 d-inline-block mx-auto" style="width: 60px;">
                      
                        <!-- Facebook -->
                        <p>
                      <a class="fb-ic">
                        <i class="fa fa-facebook-official white-text mr-4 text-light"><span class="icon_name">Facebook</span></i>
                      </a>
                      </p>
                      <!-- Twitter -->
                      <p>
                      <a class="tw-ic">
                        <i class="fa fa-twitter white-text mr-4 text-light"><span class="icon_name">Twitter</span></i>
                      </a>
                      </p>
                      <!--Linkedin -->
                      <p>
                      <a class="li-ic">
                        <i class="fa fa-linkedin white-text mr-4 text-light"><span class="icon_name">Linkedin</span></i>
                      </a>
                      </p>
                      <!--Instagram-->
                      <p></p>
                      <a class="ins-ic">
                        <i class="fa fa-instagram white-text text-light"><span class="icon_name">Instagram </span></i>
                      </a>
                      </p>
        </div>
        <!-- Grid column -->

      </div>
      <!-- Grid row -->

    </div>
    <!-- Footer Links -->


  </footer>
  <!-- Footer -->

  <script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"></script>
  <script src="https://cdn.jsdelivr.net/npm/popper.js@1.16.0/dist/umd/popper.min.js"></script>
  <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.0/js/bootstrap.min.js"></script>
    <script src="script.js"></script>

</body> <head>
