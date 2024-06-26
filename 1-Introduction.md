<!--
author:   André Dietrich; Sebastian Zug

email:    LiaScript@mail.org

version:  0.0.1

language: en

narrator: US English Female

comment:  Short Introduction on LiaScript.

import:   https://raw.githubusercontent.com/LiaTemplates/algebrite/0.2.1/README.md
          https://raw.githubusercontent.com/LiaTemplates/ABCjs/0.0.2/README.md
          https://raw.githubusercontent.com/liaTemplates/TextAnalysis/main/README.md

notranslate: <span class="notranslate">(@0)</span>

-->

[![LiaScript](https://raw.githubusercontent.com/LiaScript/LiaScript/master/badges/course.svg)](https://liascript.github.io/course/?https://github.com/LiaPlayground/eLearningAfrica-Kigali-2024/blob/main/1-Introduction.md)

# Who are we?

<iframe id="map" src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d745.0172241379928!2d13.329770317829896!3d50.92568159562554!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x47a7600bf919ad43%3A0x4dc2cb2137dcaed9!2sTechnische%20Uni%2FBergakademie%20Freibg.%20Geologisches%20Institut!5e1!3m2!1sde!2sde!4v1681986802498!5m2!1sde!2sde" style="width: 80%; height: 60vh; border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>


                                         {{1}}
| Name                    |                 eMail                   |                     Twitter                           |
| ----------------------- |:---------------------------------------:|:-----------------------------------------------------:|
| Prof. Dr. Sebastian Zug | [sebastian.zug\@informatik.tu-freiberg.de](mailto:sebastian.zug@informatik.tu-freiberg.de) |    |
| Dr. André Dietrich      | [LiaScript\@web.de](mailto:LiaScript@web.de) | [\@an_dietrich](https://twitter.com/an_dietrich) |



## Who is LiaScript?

              --{{0}}--
Hi, I am LiaScript a Markup language and interpreter for educational content.
The goal of my developers was to create a open and easy to use way to develop and distribute educational content.

![eLearning Africa Logo](https://www.elearning-africa.com/conference2023/ressources/banner/2023/social_1200_630.png)

## Features

Markdown is intended to be as easy-to-read and easy-to-write as is feasible, but unfortunately for static content only.
LiaScript is based on Markdown and extends it in various ways.


                      {{1}}
***********************************************************

__Quizzes & Surveys__

                    --{{1}}--
To our knowledge, there is no simpler way of creating quizzes and questionnaires.

Weird German articles, guess the right one for "Mädchen", which means girl:

- [( )]  male   @notranslate(der)
- [( )]  female @notranslate(die)
- [(X)]  neuter @notranslate(das)

***********************************************************


                      {{2}}
***********************************************************

__Interactive Coding__

The original goal was to create coding courses fast.
But the same principals can be used to teach writing, mathematics, and music-theory too.

```
Playing games has always been thought to be important to
the development of well-balanced and creative children;
however, what part, if any, they should play in the lives
of adults has never been researched that deeply. I believe
that playing games is every bit as important for adults
as for children. Not only is taking time out to play games
with our children and other adults valuable to building
interpersonal relationships but is also a wonderful way
to release built up tension.
```
@Textanalysis.FULL


-------------------------------------------------

```
(3 * x - 5x)^3 * (x + x)

60!
```
@Algebrite.eval


-------------------------------------------------

``` abc
% channel: 0
% autoplay: true
X:353
T: GLUECK AUF DER STEIGER KOEMMT
N: E1512
O: Europa, Mitteleuropa, Deutschland
R: Staende -, Bergmanns - Lied
M: 4/4
L: 1/16
K: G
 | G8F4A4 | G8z8 |
B8A4c4 | B8z4
G2A2 | B4B4B4A2B2 | c4A3AA4
A2B2 | c4c4c4B2c2 | d4B3BB4
A4 | G8F8 | G4e4d4
c2A2 | B8A8 | G8z8
```
@ABCJS.eval

-------------------------------------------------


***********************************************************


                      {{3}}
***********************************************************

__Multimedia__

Of course you can add any kind of multimedia content and content from other sites as well.

![Portrait of a lady](https://upload.wikimedia.org/wikipedia/commons/thumb/c/c3/Leonardo_da_Vinci_%28attrib%29-_la_Belle_Ferroniere.jpg/723px-Leonardo_da_Vinci_%28attrib%29-_la_Belle_Ferroniere.jpg "La Belle Ferronnière, c. 1490–1498")
!?[Fun with Tables](https://www.youtube.com/watch?v=Y_7q9T5jYHo)
??[Beating heart](https://sketchfab.com/3d-models/beating-heart-d9845afb1ee64ad094adc96320c67d98 "'Beating Heart' (https://skfb.ly/owVVo) by Dreamwasabducted")


***********************************************************


                      {{4}}
***********************************************************

__Animations & TextToSpeach__

                    --{{4}}--
One document can be presented in various ways.
You can use it for presentations with animation steps, read it like a textbook, or use it like an interactive screen-cast.
Just click on the presentation button to switch between modes.

***********************************************************


                      {{5}}
***********************************************************

__MORE__

                    --{{5}}--
And of course you can do much much more.


| Animal          | weight in kg | Lifespan years | Mitogen |
| --------------- | ------------:| --------------:| -------:|
| Mouse           |        0.028 |              2 |      95 |
| Flying squirrel |        0.085 |             15 |      50 |
| Brown bat       |        0.020 |             30 |      10 |
| Sheep           |           90 |             12 |      95 |
| Human           |           68 |             70 |      10 |

***********************************************************


                  {{6}}
*****************************

$a =$ <script input="range" step="1" min="-1" max="6" value="2"  output="a">@input</script>,
$b =$ <script input="range" step="0.1" min="-10" max="10" value="0"  output="b">@input</script>,
$c =$ <script modify="false" input="range" step="0.1" min="-10" max="10" value="0"  output="c">@input</script>

<script modify="false" run-once style="display: inline-block; width: 100%">
"LIASCRIPT: ### $$f(x) = x^{@input(`a`)} + x * @input(`b`) + @input(`c`)$$"
</script>

<script run-once style="display: inline-block; width: 100%">
function func(x) {
    return Math.pow(x,  @input(`a`)) + @input(`b`) * x + @input(`c`);
}

function generateData() {
    let data = [];
    for (let i = -15; i <= 15; i += 0.01) {
        data.push([i, func(i)]);
    }
    return data;
}

let option = {
    animation: false,
    grid: { top: 40, left: 50, right: 40, bottom: 50 },
    xAxis: {
        name: 'x',
        minorTick: {
            show: true
        },
        splitLine: {
            lineStyle: {
                color: '#999'
            }
        },
        minorSplitLine: {
            show: true,
            lineStyle: {
                color: '#ddd'
            }
        }
    },
    yAxis: {
        name: 'y', min: -10, max: 10,
        minorTick: {
            show: true
        },
        splitLine: {
            lineStyle: {
                color: '#999'
            }
        },
        minorSplitLine: {
            show: true,
            lineStyle: {
                color: '#ddd'
            }
        }
    },
    dataZoom: [{
        show: true,
        type: 'inside',
        filterMode: 'none',
        xAxisIndex: [0],
        startValue: -20,
        endValue: 20
    }, {
        show: true,
        type: 'inside',
        filterMode: 'none',
        yAxisIndex: [0],
        startValue: -20,
        endValue: 20
    }],
    series: [
        {
            type: 'line',
            showSymbol: false,
            clip: true,
            data: generateData()
        }
    ]
}
"HTML: <lia-chart option='" + JSON.stringify(option) + "'></lia-chart>"
</script>

*****************************

### Feature-Phone

<!--
persistent: true
-->

<video autoplay="false" id="videoElement" style="display: none; width: 100%; padding: 5px"></video>

<script input="submit" default="Open Camera">
const video = document.querySelector("#videoElement")

if (video.srcObject === null) {
    if (navigator.mediaDevices.getUserMedia) {
        navigator.mediaDevices.getUserMedia({ video: true })
            .then(function (stream) {
                video.srcObject = stream
                video.style.display = "block"
                send.lia("Close Camera")
            })
            .catch(function (error) {
                console.log("Something went wrong!")
                send.lia("Camera Problem")
            });

        send.output("Waiting for Camera")
        "LIA: wait"
    } else {
        "No Camera connected"
    }
} else {
    const tracks = video.srcObject.getTracks()
    // Stop all tracks
    tracks.forEach(track => track.stop())
    video.style.display = "none"
    video.srcObject = null
    "Open Camera"
}
</script>

## General Idea

<!--
style="width: 100%; max-width: 860px; display: block; margin-left: auto; margin-right: auto;"
-->
```ascii           Transformation of OER materials for use in various LMSs.
   +---------------------+
   | # Digital Systems V1|\
 +--------------------+  +-+
 | # Digital Systems  |\
+------------------+  +-+
| # Digital Systems|\                                      .-----------.
| (SoSe 2023)      +-+                              ╔══════|   LMS  X  |══════╗
|                    |  --------------------------> ║      '-----------'      ║
|"##" Task 1         |                              ║ Digital Systems 2023    ║
|                    |                              ║                         ║
| + Implement ...    | --------------+              ║ import numpy as np      ║
|                    |    Trans-     |              ║ ...                     ║
|                    |    formation  |              ╚═════════════════════════╝
+--------------------+               v
                                .-,(   ),-.                .-----------.
License: ...                 .-(           )-.      ╔══════|   LMS  Y  |══════╗
Content: ...                (    OER Cloud    )     ║      '-----------'      ║
Author: ...                  '-(           )-'  +-->║ Digital Systems 2023    ║
Versions: ...                   '-.(   ).-'     |   ║                         ║
                                     |          |
                                     +----------+          .-----------.
                                                |   ╔══════|  Webapp   |══════╗
                                                |   ║      '-----------'      ║
                                                +-->║ Digital Systems 2023    ║
                                                    ║                         ║
```

## Survey

### 0. Where are you from?

[[___]]

### 1. What do you expect from this tutorial?

- [[ideas]]         Ideas for own courses
- [[collaboration]] Understanding processes for collaborative course development
- [[technologies]]  Overview on web technologies / eduTech
- [[sharing]]       Methods for sharing content for free
- [[markdown]]      Get to know Markdown
- [[i18n]]          Internationalization

### 2. What tools / systems (LMS) did you use prior to create learning materials?

Separate them by comma.

   [[___]]

### 3. How would you rate your knowledge related to

Please chose a "1" for novice and "5" for expert!

   [(1)(2)(3)(4)(5)]
   [               ] Markdown
   [               ] Web development
   [               ] Git/Github

### 5. How many online course have you designed?

- [(none)] None so far
- [(< 5)]  Less than 5
- [(< 10)] Less than 10
- [(more)] More than 10
