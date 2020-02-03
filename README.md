# Front End Redesign Project for Tech Academy

## Introduction
For the final two weeks of my time at the Tech Academy I worked with several others on a project to redesign the front-end of the classroom API. Some of my tasks included creating a new nav bar, footer, buttons, etc. During the two-week sprint there were several CSS issues that cropped-up that were handled with collaboration and research. 

Below are the descriptions of the stories I worked on, as well code snippets.

## Design a new Nav Bar
The nav bar was getting complaints about it not being intuitive. I was tasked with coming-up with a whole new design and implementation. 

<head>
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css" integrity="sha384-Gn5384xqQ1aoWXA+058RXPxPg6fy4IWvTNh0E263XmFcJlSAwiGgFAW/dAiS6JXm" crossorigin="anonymous">
</head>
<nav class="navbar navbar-expand-lg navbar-custom ">
  <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
    <span class="navbar-toggler-icon"></span>
  </button>
  <div class="collapse navbar-collapse" id="navbarSupportedContent">
    <ul class="navbar-nav mr-auto">
      <li class="nav-item active">
        <a class="nav-link" href="{% url 'home' %}">The Hobby Tracker <span class="sr-only">(current)</span></a>
      </li>
      <li class="nav-item dropdown">
        <a class="nav-link dropdown-toggle" href="#" id="navbarDropdown" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
          Collections
        </a>
        <div class="dropdown-menu" aria-labelledby="navbarDropdown">
          <a class="dropdown-item" href="{% url 'footy' %}" alt="Footy Appy">Footy App</a>
          <a class="dropdown-item" href="{% url 'science' %}" alt="Science Appy">Science App</a>
          <a class="dropdown-item" href="{% url 'scoreboard' %}" alt="Lakers Scoreboard App">Lakers Scoreboard App</a>
          <a class="dropdown-item" href="{% url 'crypto' %}" alt="Crypto Currency">Crypto Currency</a>
          <a class="dropdown-item" href="" alt="">Add App</a>
          <a class="dropdown-item" href="" alt="">Add App</a>
        </div>
      </li>
    </ul>
  </div>
</nav>

body{
    background: linear-gradient(180deg, black, transparent 20%), linear-gradient(360deg, #000, transparent 20%), #090c1f      url(/static/images/bg_Yosemite.jpg) no-repeat center center fixed;
    background-size: cover;
    background-repeat: no-repeat;
}
/* ===========================================
  Navigation Bar styling  //  START
=============================================*/
.navbar-custom {
    background-color: rgba(64, 93, 135,.15)
}

.navbar-custom .navbar-nav .nav-link {
    color: rgba(152,145,128, 1);
}

.navbar-custom .nav-item.active .nav-link,
.navbar-custom .nav-item:hover .nav-link {
    color: #ffffff;

}
.navbar-custom .dropdown-menu {
    background-color: #ffffff;
}

/* ===== Navigation Bar styling  //  END =====*/
/* ===========================================


