---
layout: post
title: Jenny Mata, "Flag Project-In Process"
date: 2018-12-14
---

This week we have been working on an extension of our previous flag but instead we have been trying our best to program a more
complex flag. So far I have been planning before hand how to program the stripes and the stars with the put-image function. I have also been trying to figure out how to take the original scale numbers for the US flag and change them into numbers apropriate for the computer. A challenge that I am facing right now is thinking about how I will program 50 stars in the same way as the US flag. Since the stars aren't formed 10 rows and 5 collums but 6 stars and 5 below them until you hit 50. I plan on having a base layer of blue and adding a star to make one image with put-image. I then plan to define that image and continue with the put-image function until I have completed all 50 stars. I look forward to putting my plan in action and seeing how it turns out. The image below this post are the pieces of my flag. I first programed the pieces of the flag to later put together using only the definition names to make it easier. The star is colored black as I can't see it when it's in white or outlined black but I will change the color once I connect then blue and the star. 

```;A= 1.0    B= 1.9 -> A= 10 B= 19   A * #  B * #
; Number used A * 30 = 300  B * 30 = 570
; A/13 -> 300/13 
;6 white stripes (6 WS)
;C= 0.53 D=0.76 --> C= 5.3 D=7.6

(rectangle 570 300 "outline" "black")
(define BASE(rectangle 570 300 "outline" "black"))

(define RS(rectangle 570 23.07 "solid" "red"))
RS
RS
RS
RS
RS
RS
RS
(rectangle 570 150 "solid" "blue")
(rectangle 228 159 "solid" "blue")

;76*3 for number ^^^)
;put image function to add pieces together

(define BS(rectangle 228 159 "solid" "blue"))
BS

; FOR THE POSITION OF RS SUBTRACT 46.14 EVERY TIME 

;make two different flags, the stripes and the blue with stars; connect those two later with put image
;put-image only connects two images into one
          
(star 6 "solid" "black")
```




<style>
       
        h2 {
            color: rgb(28, 128, 128);
        }  
        
        body {
            background-color: rgb(215, 196, 255);
        }
            
        </style>   


![flagV2](/images/flagV2.png)
