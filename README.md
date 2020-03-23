<body>
    <div class="resume">
        <div id="particles-js"></div>
        <div class="image-holder">
            <img src="https://media.licdn.com/dms/image/C5103AQG5EZJtoNlW0w/profile-displayphoto-shrink_200_200/0?e=1566432000&v=beta&t=aGlWy9WgHyZXXWuEypl9OPbMieDyUVXP1NFLUQYXor4">
        </div>
        <div class="title">
            <h1>Amirul</h1>
        </div>
        <div class="navigator">
            <ul>
                <li onclick="about();">About</li>
                <li onclick="skill();">Skill</li>
                <li onclick="edu();">Education</li>
            </ul>
        </div>
        <div class="content" id="about">
            <p>I am an actuarial graduate and a graphic designer from Malaysia. Despite being an actuarial graduate, I am struggling to learn—as much as possible—all the essential skills and knowledge needed in the industry, both related and unrelated to the actuarial field, following the fourth industrial revolution.</p>
        </div>
        <div class="content" id="skill">
            <p>
                <table>
                    <tr>
                        <td onclick="js();">JavaScript</td>
                        <td onclick="java();">Java</td>
                    </tr>
                    <tr>
                        <td onclick="python();">Python</td>
                        <td onclick="r();">R</td>
                    </tr>
                    <tr>
                        <td onclick="html1();">HTML</td>
                        <td onclick="css1();">CSS</td>
                    </tr>
                </table>
            </p>
            <div class="doughnut-holder" id="chart-holder">
            
                <div class="caption"><span id="caption">JavaScript</span></div>
                <div class="doughnut" id="js"></div>
                <div class="doughnut" id="java"></div>
                <div class="doughnut" id="python"></div>
                <div class="doughnut" id="r"></div>
                <div class="doughnut1" id="html"></div>
                <div class="doughnut1" id="css"></div>
            </div>
        </div>
    </div>
    <footer>
        <p>Design by <strong>Amirul</strong></p>
    </footer>
    <script type="text/javascript" src="https://cdn.jsdelivr.net/particles.js/2.0.0/particles.min.js"></script>
    <script type="text/javascript" src="app.js"></script>
</body>
<class>
@import url('https://fonts.googleapis.com/css?family=Roboto&display=swap');

body {
    margin: 0;
    font-family: Roboto;
}

::-webkit-scrollbar {
    width: 14px;
}

::-webkit-scrollbar-thumb {
    background: #d4d4d4;
    border-radius: 10px;
}

::-webkit-scrollbar-thumb:hover {
    background: #bbbbbb;
}

.resume {
    margin: 50px auto;
    width: 360px;
    height: 640px;
    border-radius: 15px;
    box-shadow: 0px 0px 50px 0px rgba(0, 0, 0, 0.1),
    0px 0px 10px 0px rgba(0, 0, 0, 0.1);
    background: radial-gradient(rgb(255, 255, 255),
    rgba(200, 200, 200, 0.1));
}

@media (max-width: 400px) {
    .resume {
        margin: 0px auto;
    }
}
#particles-js {
    background: linear-gradient(to bottom, #4cb8c4, #3cd3ad);
    width: 100%;
    height: 140px;
    border-radius: 15px 15px 0px 0px;
    box-shadow: 0px 0px 50px 0px rgba(76, 184, 196, 0.1),
    0px 0px 5px 0px rgba(76, 184, 196, 0.8);
    transition: 0.3s;
}

#particles-js:hover {
    box-shadow: 0px 0px 60px 0px rgba(76, 184, 196, 0.1),
    0px 0px 10px 0px rgba(76, 184, 196, 0.8);
}

.image-holder {
    margin-left: 20px;
    position: relative;
    top: -120px;
    border-style: solid;
    border-color: rgba(255, 255, 255, 0.8);
    border-radius: 100%;
    border-width: 3.7px;
    box-shadow: 0px 0px 10px 0px rgba(0, 0, 0, 0.2);
    width: 140px;
    height: 140px;
    transition: 0.4s;
}

.image-holder:hover {
    top: -125px;
    box-shadow: 0px 0px 20px 0px rgba(0, 0, 0, 0.2), 0px 0px 10px 0px rgba(0, 0, 0, 0.2);
}

.image-holder img {
    border-radius: 100%;
    width: 100%;
    transform: scaleX(-1);
}

.title {
    position: relative;
    top: -220px;
    left: 185px;
    width: 0px;
}

.title h1 {
    display: inline;
    color: rgba(255, 255, 255, 0.95);
}

ul {
    list-style-type: none;
    padding: 0px;
    margin: 0px;
    text-align: center;
    position: relative;
    top: -155px;
}

li {
    display: inline;
    padding: 5px;
    color: #868686; 
}

li:hover {
    color: #3a3a3a;
    cursor: pointer;
}

li:active {
    color: gray;
}

.content {
    text-align: justify;
    margin-left: 50px;
    margin-right: 50px;
    position: relative;
    top: -150px;
    color: rgb(80, 80, 80);
    animation: animate1 1s;
    font-size: 16px;
}

@keyframes animate1 {
    0% {
        top: -90px;
        opacity: 0;
    }
    100% {
        top: -150px;
        opacity: 1;
    }
}

#skill {
    display: none;
}

table {
    margin: auto;
    border-spacing: 8px;
}

td {
    text-align: center;
    width: 100px;
    height: 50px;
    padding: 2px;
    background-color: rgba(180, 180, 180, 0.1);
    cursor: pointer;
    border-radius: 5px;
    transition: 0.15s;
}

td:hover {
    background-color: rgba(255, 255, 255, 0);
    box-shadow: 0px 0px 10px 0px rgba(0, 0, 0, 0.1), 0px 0px 3px rgba(0, 0, 0, 0.1);
    transform: scale(1.05);
}

.doughnut {
    height: 100px;
    width: 100px;
    border-style: solid;
    border-right-color: #3cd3ad;
    border-top-color: rgba(0, 0, 0, 0.1);
    border-left-color: rgba(0, 0, 0, 0.1);
    border-bottom-color: rgba(0, 0, 0, 0.1);
    border-width: 8px;
    border-radius: 100%;
    margin: auto;
    transform: rotate(-45deg);
    animation: animate2 1s;
}

.doughnut1 {
    height: 100px;
    width: 100px;
    border-style: solid;
    border-right-color: #3cd3ad;
    border-top-color: rgba(0, 0, 0, 0.1);
    border-left-color: rgba(0, 0, 0, 0.1);
    border-bottom-color: #3cd3ad;
    border-width: 8px;
    border-radius: 100%;
    margin: auto;
    transform: rotate(-45deg);
    animation: animate2 1s;
}


@keyframes animate2 {
    0% {
        transform: rotate(50deg);
    }
    50% {
        transform: rotate(-55deg);
    }
    100% {
        transform: rotate(-45deg);
    }
}

.doughnut-holder {
    display: none;
    width: 116px;
    height: 116px;
    padding: 7px;
    margin: 40px auto;
    border-radius: 500px;
    box-shadow: 0px 0px 10px 0px rgba(0, 0, 0, 0.1);
}

.caption {
    height: 0px;
    width: 100px;
    padding: 0px;
    margin: auto;
    text-align: center;
    position: relative;
    top: 40%;
}

footer p {
    color: rgba(0, 0, 0, 0.35);
    text-align: center;
}
</class>
<script>
particlesJS("particles-js",{
    "particles": {
      "number": {
        "value": 80,
        "density": {
          "enable": true,
          "value_area": 300
        }
      },
      "color": {
        "value": "#ffffff"
      },
      "shape": {
        "type": "polygon",
        "stroke": {
          "width": 0,
          "color": "#000000"
        },
        "polygon": {
          "nb_sides": 5
        },
        "image": {
          "src": "img/github.svg",
          "width": 100,
          "height": 100
        }
      },
      "opacity": {
        "value": 0.2,
        "random": false,
        "anim": {
          "enable": false,
          "speed": 1,
          "opacity_min": 0.1,
          "sync": false
        }
      },
      "size": {
        "value": 2.5,
        "random": true,
        "anim": {
          "enable": false,
          "speed": 40,
          "size_min": 0.1,
          "sync": false
        }
      },
      "line_linked": {
        "enable": true,
        "distance": 100,
        "color": "#ffffff",
        "opacity": 0.4,
        "width": 1
      },
      "move": {
        "enable": true,
        "speed": 2,
        "direction": "none",
        "random": false,
        "straight": false,
        "out_mode": "out",
        "bounce": false,
        "attract": {
          "enable": false,
          "rotateX": 600,
          "rotateY": 1200
        }
      }
    },
    "interactivity": {
      "detect_on": "canvas",
      "events": {
        "onhover": {
          "enable": true,
          "mode": "grab"
        },
        "onclick": {
          "enable": true,
          "mode": "push"
        },
        "resize": true
      },
      "modes": {
        "grab": {
          "distance": 121,
          "line_linked": {
            "opacity": 0.5
          }
        },
        "bubble": {
          "distance": 400,
          "size": 40,
          "duration": 2,
          "opacity": 8,
          "speed": 3
        },
        "repulse": {
          "distance": 97,
          "duration": 0.4
        },
        "push": {
          "particles_nb": 4
        },
        "remove": {
          "particles_nb": 2
        }
      }
    },
    "retina_detect": true
  });

  function e(id) {
    return document.getElementById(id);
  }

  function about() {
    e("about").style.display = 'block';
    e("skill").style.display = 'none';
    e("chart-holder").style.display = 'none';
  }

  function skill() {
    e("skill").style.display = 'block';
    e("about").style.display = 'none';
  }

  function js() {
    e("chart-holder").style.display = 'block';
    e("js").style.display = 'block';
    e("java").style.display = 'none';
    e("python").style.display = 'none';
    e("r").style.display = 'none';
    e("html").style.display = 'none';
    e("css").style.display = 'none';
    e("caption").innerHTML = 'JavaScript';
  }

  function java() {
    e("chart-holder").style.display = 'block';
    e("js").style.display = 'none';
    e("java").style.display = 'block';
    e("python").style.display = 'none';
    e("r").style.display = 'none';
    e("html").style.display = 'none';
    e("css").style.display = 'none';
    e("caption").innerHTML = 'Java';
  }

  function python() {
    e("chart-holder").style.display = 'block';
    e("js").style.display = 'none';
    e("java").style.display = 'none';
    e("python").style.display = 'block';
    e("r").style.display = 'none';
    e("html").style.display = 'none';
    e("css").style.display = 'none';
    e("caption").innerHTML = 'Python';
  }

  function r() {
    e("chart-holder").style.display = 'block';
    e("js").style.display = 'none';
    e("java").style.display = 'none';
    e("python").style.display = 'none';
    e("r").style.display = 'block';
    e("html").style.display = 'none';
    e("css").style.display = 'none';
    e("caption").innerHTML = 'R';
  }

  function html1() {
    e("chart-holder").style.display = 'block';
    e("js").style.display = 'none';
    e("java").style.display = 'none';
    e("python").style.display = 'none';
    e("r").style.display = 'none';
    e("html").style.display = 'block';
    e("css").style.display = 'none';
    e("caption").innerHTML = 'HTML';
  }

  function css1() {
    e("chart-holder").style.display = 'block';
    e("js").style.display = 'none';
    e("java").style.display = 'none';
    e("python").style.display = 'none';
    e("r").style.display = 'none';
    e("html").style.display = 'none';
    e("css").style.display = 'block';
    e("caption").innerHTML = 'CSS';
  }
</script>
