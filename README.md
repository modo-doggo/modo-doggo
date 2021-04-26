- 👋 Hi, I’m @modo-doggo
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
modo-doggo/modo-doggo is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
import time


PT =int(input("Number of seconds (dont go over 59)"))  
PT2 =int(input("Number of minutes (dont go over 59)"))  
PT3 =int(input("Number of hours (dont go over 12)"))

#########################
seconds = PT

minutes = PT2

hours = PT3



     
import turtle
screen = turtle.Screen()
screen.setup(500,500)
t1 = turtle.Turtle()
t1.color("red")
t1.up()
t1.goto(-100,8)
t1.hideturtle()


############ Turtle 2 ######################
t2 = turtle.Turtle( )
#t2.up()
t2.begin_fill() 
t2.goto(-200,50)
t2.speed(10)	
t2.width(6)
t2.forward(200)
t2.right(90)
t2.forward(65)
t2.right(90)
t2.forward(200)
t2.right(90)
t2.forward(65)
t2.end_fill()
t2.hideturtle()





clock_working = "true" 
while clock_working == "true":
     print( str(hours).zfill(2) + " hours and " + str(minutes).zfill(2) + " minutes and " + str(seconds).zfill(2) + " seconds")
     t1.write(str(hours).zfill(2) + ":" + str(minutes).zfill(2) + ":" + str(seconds).zfill(2) + "" ,align = "center", font = ("Times New Roman",25,"bold"))   
     seconds = seconds + 1
     time.sleep(1) 
     if seconds == 60:
          minutes = minutes + 1
          seconds = 0
          ############   Hours   #################

     if minutes == 60:
          hours = hours + 1
          minutes = 0
    
    
     if hours == 13:
          hours = hours + 1
          hours = 1
    
     t1.clear()






