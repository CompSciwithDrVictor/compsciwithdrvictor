---
permalink: /
title: "Welcome!"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

My name is Victor and I'm a PhD in Systems Design Engineering. I'm currently a Lecturer in the [School of Computing Science](https://www.sfu.ca/computing.html) at [Simon Fraser University](https://www.sfu.ca/). I specialize in Human-Computer Interaction & Design and Emerging Technologies like tangible user interfaces and wearables. My day job is teaching Computer Science courses and I have been doing this for over 10 years.

I have accumulated a lot of knowledge and skills while teaching CS courses and would like to use this website to share some of those with you! Some of them are related to the courses I'm teaching and some are more general to the broader area of CS. If you want to learn something about CS you've come to the right place!

Thanks for stopping by and if you like my content please bookmark this website! Also share it with your friends who might find it helpful!

Also check out my [YouTube Channel](https://www.youtube.com/@CompSciwithDrVictor)!

What's New
======
I'm adding new content to this website regularly. Some of the things include:
- Teaching (this will be my main focus here, refer to the next section for more details).
- Blog Posts of random thoughts.
- Publications (as a teaching faculty I don't publish in my usual research venues as much as before, but hopefully I'll be publishing in other channels like education conferences and web platforms).
- ... and more.

Why This Website
======
The main motivation for me to create this website is that I realized many of the course materials I create become inaccessible after the term ends, due to the set up of the LMS of my University. And I want my students (and also those who are interested) to be able to access in particular the supplementary reading anytime. My goal (at least for now) is not to put everything here, as there are some current-student-only materials that I want to keep at the LMS. Instead, I want to put something that I want my students to continue to explore after the courses to explore more and/or refer back to some of the topics mentioned in the courses.

GitHub Pages seem to be a good place to do this because it's more flexible and it many ways easier to setup/maintain. Also, many academics and developers are moving their content here, which means a bigger community and better support. Moreover, this is the first time I set up a website like this, so it'll be a fun experience for me too.

A Little Fun Script to Tell Time
------
<font id="timeString">It's now <font color="#afafaf">zero</font> minute until <font color="#afafaf">zero</font> in the midnight.</font>
<script>
//reference: rossgoodwin.com/clock

var numToText = 
[ "zero", "one", "two", "three", "four", "five", "six", "seven", "eight", "nine", "ten", "eleven", "twelve", "thirteen", "fourteen", "fifteen", "sixteen", "seventeen", "eighteen", "nineteen", "twenty" ];

var fontTagFront = "<font color=\"afafaf\">";
var fontTagBack = "</font>";

function startTime() {
        var today = new Date();
        var h = today.getHours();
        var m = today.getMinutes();
        document.getElementById("timeString").innerHTML = "It\'s now ";
        if (m === 0) {//it's the o'clock
                document.getElementById("timeString").innerHTML += ctt0(h, m);
        } else if (m > 0 && m < 15) {
                document.getElementById("timeString").innerHTML += ctt1(h, m);
        } else if (m === 15) {//it's the quarter-past
                document.getElementById("timeString").innerHTML += ctt2(h, m);
        } else if (m > 15 && m < 30) {
                document.getElementById("timeString").innerHTML += ctt3(h, m);
        } else if (m === 30) {//it's the half-past
                document.getElementById("timeString").innerHTML += ctt4(h, m);
        } else if (m > 30 && m < 45) {
                document.getElementById("timeString").innerHTML += ctt3(h, m);
        } else if (m === 45) {//it's the quarter-to
                document.getElementById("timeString").innerHTML += ctt6(h, m);
        } else if (m > 45 && m <= 49) {
                document.getElementById("timeString").innerHTML += ctt3(h, m);
        } else {
                document.getElementById("timeString").innerHTML += ctt8(h, m);
        }
        document.getElementById("timeString").innerHTML += ".";
}

//the o'clock case
function ctt0(hour, minute) {
        var timeStr = "";

        if (hour === 0) {
                timeStr = "midnight";
        } else if (hour === 12) {
                timeStr = "noon";
        } else {
                var hr = hour;
                if (hour > 12) {
                        hr = hour - 12;
                }
                timeStr += fontTagFront + numToText[hr] + fontTagBack;
        }

        //neither midnight nor noon
        if (hour != 0 && hour != 12) {
                timeStr += " o\'clock";
                
                if (hour < 12) {
                        timeStr += " in the morning";
                } else if (hour > 17) {
                        timeStr += " in the evening";
                } else {
                        timeStr += " in the afternoon";
                }
        }

        return timeStr;
}

//the x-minutes-past-hour case
function ctt1(hour, minute) {
        var timeStr = "";
        
        //timeStr += minute;
        if (minute <= 20) {
                timeStr += fontTagFront + numToText[minute] + fontTagBack;
         } else if (minute < 30) {
                timeStr += fontTagFront + "twenty-"+numToText[minute%10] + fontTagBack;
         } else if (minute === 30) {
                timeStr += fontTagFront + "thirty" + fontTagBack;
         } else if (minute < 40) {
                timeStr += fontTagFront + "thirty-"+numToText[minute%10] + fontTagBack;
         } else if (minute === 40) {
                timeStr += fontTagFront + "forty" + fontTagBack;
         } else if (minute < 50) {
                timeStr += fontTagFront + "forty-"+numToText[minute%10] + fontTagBack;
         } else if (minute === 50) {
                timeStr += fontTagFront + "fifty" + fontTagBack;
         } else {
                timeStr += fontTagFront + "fifty-"+numToText[minute%10] + fontTagBack;
         }

        if (minute === 1) {//singular
                timeStr += " minute";
        } else {//plural
                timeStr += " minutes";
        }

        if (Math.random() >= 0.5) {
                timeStr += " past";
        } else {
                timeStr += " after";
        }

        if (hour === 0) {//midnight
                timeStr += " midnight";
        } else if (hour === 12) {//noon
                timeStr += " noon";
        } else {
                var hr = hour;
                if (hour > 12) {
                        hr = hour - 12;
                }
                timeStr += fontTagFront + " " + numToText[hr] + fontTagBack;
        }

        if (hour != 0 && hour != 12) {
                if (hour < 12) {
                        timeStr += " in the morning";
                } else if (hour > 17) {
                        timeStr += " in the evening";
                } else {
                        timeStr += " in the afternoon";
                }
        }
        
        return timeStr;
}

//the quarter-past-hour case
function ctt2(hour, minute) {
        var timeStr = "";

        timeStr += fontTagFront + "a quarter" + fontTagBack;

        if (Math.random() >= 0.5) {
                timeStr += " past";
        } else {
                timeStr += " after";
        }

        if (hour === 0) {
                timeStr += " midnight"; 
        }
        else if (hour === 12) {
                timeStr += " noon";
        }
        else {
                var hr = hour;
                if (hour > 12) {
                        hr = hour - 12;
                }
                timeStr += fontTagFront + " " + numToText[hr] + fontTagBack;
        }

        if (hour != 0 && hour != 12) {

                if (hour < 12) {
                        timeStr += " in the morning";
                } 
                else if (hour > 17) {
                        timeStr += " in the evening";
                }
                else {
                        timeStr += " in the afternoon";
                }
        }

        return timeStr;
}

//the hour-minute case
function ctt3(hour, minute) {
        var timeStr = "";

        var hr = hour;
        if (hour === 0) {
                hr = 12;
        } else if (hour > 12) {
                hr = hour - 12;
        }
        timeStr += fontTagFront + numToText[hr] + fontTagBack;

        if (minute <= 20) {
                timeStr += fontTagFront + " " + numToText[minute] + fontTagBack;
         } else if (minute < 30) {
                timeStr += fontTagFront + " twenty-"+numToText[minute%10] + fontTagBack;
         } else if (minute === 30) {
                timeStr += fontTagFront + " thirty" + fontTagBack ;
         } else if (minute < 40) {
                timeStr += fontTagFront + " thirty-"+numToText[minute%10] + fontTagBack;
         } else if (minute === 40) {
                timeStr += fontTagFront + " forty" + fontTagBack;
         } else if (minute < 50) {
                timeStr += fontTagFront + " forty-"+numToText[minute%10] + fontTagBack;
         } else if (minute === 50) {
                timeStr += fontTagFront + " fifty" + fontTagBack;
         } else {
                timeStr += fontTagFront + " fifty-"+numToText[minute%10] + fontTagBack;
         }

        if (hour != 0 && hour != 12) {
                if (hour < 12) {
                        timeStr += " in the morning";
                } 
                else if (hour > 17) {
                        timeStr += " in the evening";
                }
                else {
                        timeStr += " in the afternoon";
                }
        }
        else {
                if (hour === 0) {
                        timeStr += " ante meridiem";
                } 
                else if (hour === 12) {
                        timeStr += " post meridiem";
                }
        }

        return timeStr;
}

//the half-past case
function ctt4(hour, minute) {
        var timeStr = "";

        timeStr += fontTagFront + "half past" + fontTagBack;

        if (hour === 0) {
                timeStr += " midnight";    
        }
        else if (hour === 12) {
                timeStr += " noon";
        }
        else {
                var hr = hour;
                if (hour > 12) {
                        hr = hour - 12;
                }
                timeStr += fontTagFront + " " + numToText[hr] + fontTagBack;
        }

        if (hour != 0 && hour != 12) {

                if (hour < 12) {
                        timeStr += " in the morning";
                } 
                else if (hour > 17) {
                        timeStr += " in the evening";
                }
                else {
                        timeStr += " in the afternoon";
                }
        }

        return timeStr;
}

//the quater-to-hour case
function ctt6(hour, minute) {
        var timeStr = "";

        timeStr += fontTagFront + "a quarter" + fontTagBack;

        if (Math.random() >= 0.5) {
                timeStr += " until";
        } else {
                timeStr += " to";
        }

        if (hour === 11) {
                timeStr += " noon";
        }
        else if (hour === 23) {
                timeStr += " midnight";
        }
        else {
                var hr = hour + 1;
                if (hour > 11) {
                        hr = hour - 11;
                }
                timeStr += fontTagFront + " " + numToText[hr] + fontTagBack;

                if (hour <= 10) {
                        timeStr += " in the morning";
                } else if (hour >= 17) {
                        timeStr += " in the evening";
                } else {
                        timeStr += " in the afternoon";
                }
        }

        return timeStr;
}

//the x-minutes-to-hour case
function ctt8(hour, minute) {
        var timeStr = "";

        timeStr += fontTagFront + numToText[(60-minute)] + fontTagBack;

        if (minute === 59) {
                timeStr += " minute";
        } else {
                timeStr += " minutes";
        }

        if (Math.random() >= 0.5) {
                timeStr += " until";
        } else {
                timeStr += " to";
        }

        if (hour === 11) {
                timeStr += " noon";
        }
        else if (hour === 23) {
                timeStr += " midnight";
        }
        else {
                var hr = hour + 1;
                if (hour > 11) {
                        hr = hour - 11;
                }
                timeStr += fontTagFront + " " + numToText[hr] + fontTagBack;

                if (hour <= 10) {
                        timeStr += " in the morning";
                } else if (hour >= 17) {
                        timeStr += " in the evening";
                } else {
                        timeStr += " in the afternoon";
                }
        }

        return timeStr;
}

//iterate and update time if the minute is changed
function checkMinute() {
        var minute = new Date().getMinutes();
        if (minute != currentMinute) {
                currentMinute = minute;
                startTime();
        }
}

//set the minute when the page loads
var currentMinute = new Date().getMinutes();

(function() {
        startTime();
        setInterval(checkMinute, 5000); //run every 5 sec
} ());

</script>