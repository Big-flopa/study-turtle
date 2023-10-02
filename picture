import turtle
import math


screen = turtle.Turtle()
screen.getscreen().setup(750,750)
screen.hideturtle()


def sky(x,y):
    # рисует небо
    sky = turtle.Turtle()
    sky.penup()
    sky.speed(0)
    sky.pencolor("blue")
    sky.fillcolor("blue")
    sky.hideturtle()
    sky.goto(x,y)
    sky.pendown()
    sky.begin_fill()
    sky.goto(x,y+300)
    sky.goto(x+970,y+300)
    sky.goto(x+1270,y)
    sky.goto(x,y)
    sky.end_fill()  

def mountain(x,y):
    # эта функция рисует гору
    mtn = turtle.Turtle()
    mtn.hideturtle()
    mtn.pencolor("white")
    mtn.speed(0)
    mtn.penup()
    mtn.goto(x,y)
    mtn.fillcolor("gray")
    mtn.begin_fill()
    mtn.pendown()
    mtn.goto(x-100,y)
    mtn.goto(x,y+150)
    mtn.goto(x+100,y)
    mtn.goto(x,y)
    mtn.end_fill()

def tringel(x,y):
    # эта функция рисует триугольник
    tringel = turtle.Turtle()
    tringel.hideturtle()
    tringel.pencolor("green")
    tringel.speed(0)
    tringel.penup()
    tringel.goto(x,y)
    tringel.fillcolor("green")
    tringel.begin_fill()
    tringel.pendown()   
    tringel.goto(x-20,y)
    tringel.goto(x,y+20)
    tringel.goto(x+20,y)
    tringel.goto(x,y)
    tringel.end_fill()
    
def stem(x,y):
    # эта функция рисует ствол
    stem = turtle.Turtle()
    stem.hideturtle()
    stem.pencolor("brown")
    stem.speed(0)
    stem.penup()
    stem.goto(x,y)
    stem.fillcolor("brown")
    stem.begin_fill()
    stem.pendown()
    
    stem.goto(x-5,y)
    stem.goto(x-5,y-15)
    stem.goto(x+5,y-15)
    stem.goto(x+5,y)
    stem.goto(x,y)
    stem.end_fill()
    
def leaf(x,y):
    # рисует листву
    for _ in range(1):
        tringel(x,y)
        y += 150

def tree(x,y):
    # рисует дерево
    stem(x, y)
    tringel(x,y)
    
def trees_vertical(x,y):
    # рисует деревья в ряд
    for _ in range(4):
        tree(x,y)
        x+=15
        y-=10
        
def trees_horizontal(x,y):
    # рисует ряд деревьев по гаризантали
    for _ in range(8):
        trees_vertical(x,y)
        x-=100

def mountains(x,y):
    # рисует горы в ряд
    for _ in range(7):
        mountain(x,y)
        x+= 100

def cloud(x,y):
    # эта функция рисует облака
    cloud = turtle.Turtle()
    cloud.hideturtle()
    cloud.speed(0)
    cloud.penup()
    cloud.pencolor("gray")
    cloud.goto(x,y)
    cloud.pendown()
    cloud.fillcolor("gray")
    cloud.begin_fill()
    cloud.left(55)
    for i in range(15):
        cloud.forward(2)
        cloud.right(4)
    cloud.left(80)
    for i in range(45):
        cloud.forward(2)
        cloud.right(4)
    cloud.goto(x,y)
    cloud.end_fill() 
    
def clouds(x,y):
    # рисует облака
    for _ in range(3):
        cloud(x,y)
        x+=300

# рисуем общую картину
sky(-370,100)
clouds(-350,250)
clouds(-200,300)
mountains(-350,125)
mountains(-300,100)
trees_horizontal(+330,+90)

turtle.done()
