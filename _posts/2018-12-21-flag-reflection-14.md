---
layout: post
title: "Flag Project - Final Submission"
date: 2018-12-21
---

## Flag of _United States_ by _Jenny Mata_

## Describe your program

-   I designed the flag of the United States 
-   I'd expect a 3 as I did not incorparate some of the components Mr. Allatta was hoping for in my program. Such as 
definition funtions and using a definition and having the computer do the math for me instead of me having to do it. I think 
that I deserve this grade as I also struggled a little bit in making my flag and I'm guessing it's because I missed a day of
class and since I don't know what we learned that day I don't know if I missed something important.



## Current output


* * *
![FlagVer2](/images/FlagVer2.png)
* * *

## Describe your process.


My questions for my flag is how to scale the distance of the stars because I got stuck on doing the star's positions from eachother instead of just continuing with it. I struggled with this because I wanted my flag to be at it's best when scaled.I didn't have much of a strategy, I just went along with what I was doing. 


## Explain your code.


* * *

```
(define WIDTH 570)
(define LENGTH 300)
(define WIDTH2 228)
(define LENGTH2 159)
(define BASE(rectangle WIDTH LENGTH "solid" "white"))
(define old-glory-red(make-color 187 19 62))
(define old-glory-blue(make-color 0 38 100))
(define RS(rectangle WIDTH (/ 300 13) "solid" old-glory-red))
(define BR(rectangle WIDTH2 LENGTH2 "solid" old-glory-blue))
(define 1S(star 6 "solid" "white"))
(define S(scale 1.7 1S))
```

* * *

 
-  This program that I chose begins with the arguments defining the width and lengths of both the wntire flag and the blue rectangle of the US flag. Then going on to the colors needed for the US flag with and next with the size of the red stripes included in the US flag. The code I posted are the most significant to my program as it starts of the definitions of my program so I can be able to shorten my code as to repeeating the same numbers and code many times. This code works both independently and along with the rest of the program because of this reason. In order to prevent a lot of irrelevant repetitions of the same code. 

## Program code

```
(define WIDTH 570)
(define LENGTH 300)
(define WIDTH2 228)
(define LENGTH2 159)
(define BASE(rectangle WIDTH LENGTH "solid" "white"))
(define old-glory-red(make-color 187 19 62))
(define old-glory-blue(make-color 0 38 100))
(define RS(rectangle WIDTH (/ 300 13) "solid" old-glory-red))
(define BR(rectangle WIDTH2 LENGTH2 "solid" old-glory-blue))
;FOR THE POSITION OF RS SUBTRACT 42.6 EVERYTIME
(define 1S(star 6 "solid" "white"))
(define S(scale 1.7 1S))
(define RSF1(put-image RS 285 287 BASE))

(define RSF2(put-image RS 285 240.86(put-image RS 285 287 BASE)))

(define RSF3(put-image RS 285 194.72(put-image RS 285 240.86(put-image RS 285 287 BASE))))

(define RSF4(put-image RS 285 148.58 RSF3))
(define RSF5(put-image RS 285 102.44 RSF4))
(define RSF6(put-image RS 285 56.3 RSF5))
(define RSF7(put-image RS 285 10.16 RSF6))
(define Star1(put-image S 18 144 BR))
(define Star2(put-image S 60 144 Star1))
(define Star3(put-image S 102 144 Star2))
(define Star4(put-image S 144 144 Star3))
(define Star5(put-image S 186 144 Star4))
(define Star6(put-image S 228 144 Star5))



(define US-FLAG-IN-PROGRESS(put-image Star6 115 219 RSF7))
US-FLAG-IN-PROGRESS

;A= 1.0    B= 1.9 -> A= 10 B= 19   A * #  B * #
; Number used A * 30 = 300  B * 30 = 570
; A/13 -> 300/13 
;6 white stripes (6 WS)
;C= 0.53 D=0.76 --> C= 5.3 D=7.6

```

<style>
       
        h2 {
            color: rgb(28, 128, 128);
        }  
        
        body {
            background-color: rgb(215, 196, 255);
        }
            
        </style>   
