<!DOCTYPE html>
<html>
<title>Parke Loyd</title>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<link rel="stylesheet" href="https://www.w3schools.com/w3css/4/w3.css">
<link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Lato">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
<style>
body,h1,h2,h3,h4,h5,h6 {font-family: "Lato", sans-serif;}
body, html {
  height: 100%;
  color: #777;
  line-height: 1.8;
}

/* Create a Parallax Effect */
.bgimg-1, .bgimg-2, .bgimg-3 {
  background-attachment: fixed;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}

/* First image (Logo. Full height) */
.bgimg-1 {
  background-image: url('images/banner.jpg');
  min-height: 100%;
}

/* Second image (Portfolio) */
.bgimg-2 {
  background-image: url("images/research.jpg");
  min-height: 400px;
}

/* Third image (Contact) */
.bgimg-3 {
  background-image: url("images/wildastro.jpg");
  min-height: 400px;
}

.w3-wide {letter-spacing: 10px;}
.w3-hover-opacity {cursor: pointer;}

/* Turn off parallax scrolling for tablets and phones */
@media only screen and (max-device-width: 800px) {
  .bgimg-1, .bgimg-2, .bgimg-3 {
    background-attachment: scroll;
    min-height: 400px;
  }
}

/* Code I added for uneven columns */
.left-slim-col {
    width: 33%;
    padding: 0 10px 0 0;
    float: left;
}

.right-fat-col {
    width: 66%;
    padding: 0 10px 0 0;
    float: right;
}

/* Stack columns on small screens */
@media only screen and (max-width: 800px) {

   .left-slim-col {
        width: 100%;
        padding-bottom: 10px;
        float: none;
    }

    .right-fat-col {
        width: 100%;
        padding-bottom: 10px;
        float: none;
    }

}

</style>
<body>

<!-- Navbar (sit on top) -->
<div class="w3-top">
  <div class="w3-bar" id="myNavbar">
    <a class="w3-bar-item w3-button w3-hover-black w3-hide-medium w3-hide-large w3-right" href="javascript:void(0);" onclick="toggleFunction()" title="Toggle Navigation Menu">
      <i class="fa fa-bars"></i>
    </a>
    <a href="#home" class="w3-bar-item w3-button">HOME</a>
    <a href="#about" class="w3-bar-item w3-button w3-hide-small"><i class="fa"></i> ABOUT</a>
    <a href="#research" class="w3-bar-item w3-button w3-hide-small"><i class="fa"></i> RESEARCH</a>
    <a href="#wildastro" class="w3-bar-item w3-button w3-hide-small"><i class="fa"></i> WILD ASTRO CLASS</a>
    <a href="#contact" class="w3-bar-item w3-button w3-hide-small"><i class="fa"></i> CONTACT</a>
    <a href="#" class="w3-bar-item w3-button w3-hide-small w3-right w3-hover-red">
    </a>
  </div>

  <!-- Navbar on small screens -->
  <div id="navDemo" class="w3-bar-block w3-white w3-hide w3-hide-large w3-hide-medium">
    <a href="#about" class="w3-bar-item w3-button" onclick="toggleFunction()">ABOUT</a>
    <a href="#research" class="w3-bar-item w3-button" onclick="toggleFunction()">RESEARCH</a>
    <a href="#wildastro" class="w3-bar-item w3-button" onclick="toggleFunction()">WILDASTRO</a>
    <a href="#contact" class="w3-bar-item w3-button" onclick="toggleFunction()">CONTACT</a>
  </div>
</div>

<!-- First Parallax Image with Logo Text -->
<div class="bgimg-1 w3-display-container w3-opacity-min" id="home">
  <div class="w3-display-middle" style="white-space:nowrap;">
    <span class="w3-center w3-padding-large w3-black w3-xlarge w3-wide w3-animate-opacity">R. O. PARKE LOYD</span>
  </div>
</div>

<!-- Container (About Section) -->
<div class="w3-content w3-container w3-padding-64" id="about">
  <h3 class="w3-center">ABOUT ME</h3>
  <div class="w3-row">
    <hr>
    <div class="left-slim-col m6 w3-center w3-padding-large">
      <img src="images/me.jpg" class="w3-round w3-image w3-hover-opacity-off" alt="Portrait" width=100%>
    </div>

    <div class="right-fat-col m6 w3-padding-large">
      <p>Hi, I’m Parke! I’m an astrophysicist currently working with <a style="text-decoration:none" href=http://www.evgenyashkolnik.com>Evgenya Shkolnik</a>'s group at Arizona State University. I research planetary systems with stars smaller than the Sun, focusing on the space environment these stars provide to their planets. Yearly, I co-instruct a class called <a style="text-decoration:none" href="#wildastro">Wilderness Astronomy</a> that I created with fellow astro-outdoorsperson <a style="text-decoration:none" href=http://melodiekao.com>Melodie Kao</a>. In the odds and ends of my time, I climb cliffs, wander through wildernesses, <a style="text-decoration:none" href=http://hl-treefarm.com>cultivate evergreen trees</a>, and putter around in <a style="text-decoration:none" href="https://www.instagram.com/n721p/">my little plane</a>. All these things are joined by one grand theme: a love for the feeling of being overcome with awe, whether through imagining alien worlds, soaring in an endless sea of air, clinging to the face of a mountain, or disappearing into a vast wilderness.</p>
      <p><a href="https://docs.google.com/document/d/1PyoDjpPQu-yY0I2roMUrVg6DDLK4_Sc2Jkqy_CmEsnA/export?format=pdf">Curriculum Vitae (CV)</a>
    </div>
</div>
<hr>

<!-- Second Parallax Image with Research Text -->
<div class="bgimg-2 w3-display-container w3-opacity-min" id="research">
  <div class="w3-display-middle">
    <span class="w3-xxlarge w3-text-white w3-wide">RESEARCH</span>
  </div>
</div>

<!-- Container (Research Section) -->
<div class="w3-content w3-container w3-padding-64">
  <h3 class="w3-center">RESEARCH</h3>
  <hr>
  <p class="w3-center"><a href="https://ui.adsabs.harvard.edu/#/public-libraries/Auik-C1CQ5uDKSMtgZb-XA">Publication List</a> (<a href="https://ui.adsabs.harvard.edu/#/public-libraries/e5y_8q3hQPuGeDzEAYaSvA">Refereed</a>) | <a href="https://orcid.org/0000-0001-5646-6668">ORCID 0000-0001-5646-6668</a> | <a href="http://github.com/parkus">GitHub Code</a></p>
  <p>My research focuses on low-mass stars and their planets. No planetary systems are more numerous or longer lived than those with low mass stars. I work to characterize the environments these stars provide for their planets over their lifetimes. This includes exploring methods to observationally constrain stellar space weather, especially coronal mass ejections. On the planetary side of my research, I recently published an attempt to empirically test if the scarcity of planets with radii near 1.8x Earth's could be a direct result of atmospehric erosion by stellar radiation. (My test and those others have published remain inconclusive.) In the past, I have contributed to observations of planets actively blowing off their atmospheres under the intense radiation of their host star, and I hope to conduct similar observations in coming years to learn more about planetary atmospheric escape.</p>
  <p class="w3-center"><em>If searching for my publications, note that online databases sometimes mistake my last name as "Parke Loyd" instead of simply "Loyd."</em></p>
  <hr>
</div>

<!-- Second Parallax Image with wildastro Text -->
<div class="bgimg-3 w3-display-container w3-opacity-min" id="wildastro">
  <div class="w3-display-middle">
    <span class="w3-xxlarge w3-text-white w3-wide">WILD ASTRO</span>
  </div>
</div>

<!-- Container (wilastro Section) -->
<div class="w3-content w3-container w3-padding-64">
  <h3 class="w3-center">WILDERNESS ASTRONOMY COURSE</h3>
  <hr>
  <p class="w3-center"><a href="https://studyabroad.asu.edu/?go=wildernessastronomy">ASU Course Brochure for Wilderness Astronomy</a>
  <p>In 2019, I teamed up with fellow astrophysicist and wilderness backpacker <a href="http://melodiekao.com">Melodie Kao</a> to create the outdoor learning course Wilderness Astronomy that we now offer annually. In this introductory undergraduate level course, we lead students on a week-long backpacking trip in the otherworldly backcountry terrain of Arizona. What they see and feel as they hike becomes a canvas for teaching planetary science, and what they see in the dark, unpolluted skies at night becomes a canvas for teaching astronomy. This is an impactful way to learn planetary science and astronomy. However, our goals reach beyond instilling facts and concepts. We want students who feel curious but intimidated to realize they have the capacity and agency to engage in both a physical exploration of our planet and an intellectual exploration of the cosmos. Meanwhile, we hope that we leave with them indelible memories of awe-inspring experiencies that are tied to "aha" moments about how planets, stars, and the cosmos work.</p>
    <p>The course was recently featured in <a href="https://asunow.asu.edu/20191219-discoveries-explore-stars-—-and-wilderness">an article by ASU Now</a>.</p>
    <hr>
</div>

<!-- Container (Contact Section) -->
<div class="w3-content w3-container w3-padding-64" id="contact">
  <h3 class="w3-center">CONTACT</h3>
  <p class="w3-center"><a href="mailto:parke@asu.edu">parke@asu.edu</a></p>
</div>

<!-- Footer -->
<footer class="w3-center w3-black w3-padding-64 w3-opacity w3-hover-opacity-off">
  <a href="#home" class="w3-button w3-light-grey"><i class="fa fa-arrow-up w3-margin-right"></i>To the top</a>
  <p>Powered by <a href="https://www.w3schools.com/w3css/default.asp" title="W3.CSS" target="_blank" class="w3-hover-text-green">w3.css</a></p>
</footer>

<script>
// Modal Image Gallery
function onClick(element) {
  document.getElementById("img01").src = element.src;
  document.getElementById("modal01").style.display = "block";
  var captionText = document.getElementById("caption");
  captionText.innerHTML = element.alt;
}

// Change style of navbar on scroll
window.onscroll = function() {myFunction()};
function myFunction() {
    var navbar = document.getElementById("myNavbar");
    if (document.body.scrollTop > 100 || document.documentElement.scrollTop > 100) {
        navbar.className = "w3-bar" + " w3-card" + " w3-animate-top" + " w3-white";
    } else {
        navbar.className = navbar.className.replace(" w3-card w3-animate-top w3-white", "");
    }
}

// Used to toggle the menu on small screens when clicking on the menu button
function toggleFunction() {
    var x = document.getElementById("navDemo");
    if (x.className.indexOf("w3-show") == -1) {
        x.className += " w3-show";
    } else {
        x.className = x.className.replace(" w3-show", "");
    }
}
</script>

</body>
</html>
