# chrome-logo
#chrome logo using python turtle


#Here is the code :
from turtle import *
from time import sleep
bgcolor('black')
colormode(255)
red=(223, 35, 35); green=(75, 183, 75); yellow= (252, 210, 9);
blue=(86, 146, 195) # with Gimp
r=120
speed(2)
seth(-150)
up()
#  ------------- The red petal ----------------------
color(red)
begin_fill()
fd(r)
down()
right(90)
circle(-r, 120)
fd(r*3**.5)
left(120)
circle(2*r, 120)
left(60)
fd(r*3**.5)
end_fill()
#  ------------- The green petal ----------------------
left(180)
color(green)
begin_fill()
fd(r*3**.5)
left(120)
circle(2*r, 120)
left(60)
fd(r*3**.5)
left(180)
circle(-r, 120)
end_fill()
#  ------------- The yellow petal ----------------------
left(180)
circle(r, 120)
color(yellow)
begin_fill()
circle(r, 120)
right(180)
fd(r*3**.5)
right(60)
circle(-2*r, 120)
right(120)
fd(r*3**.5)
end_fill()
#  ------------- The blue disk ----------------------
up()
left(90)
fd(r/20)
seth(60)
color(blue)
down()
begin_fill()
circle(distance(0,0))
end_fill()
ht()
sleep(0.8)
#  ------------- Last ----------------------
screen=getscreen()
screen.register_shape("chrome")
clear()
ht()
up()
goto(-300, 0)
shape("chrome")
st()
down()
goto(0,0)
color("black")
write("@Bharath.coder", font=("Arial", 30, "bold"))
goto(280, 0)









