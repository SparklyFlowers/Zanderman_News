[![Run on Repl.it](https://repl.it/badge/github/SparklyFlowers/Zanderman_News)](https://repl.it/github/SparklyFlowers/Zanderman_News)
#logo
import time
import turtle
wn = turtle.Screen()
wn.screensize(1000, 1000)
john = turtle.Turtle()
john.hideturtle()
john.penup()
def undo (times, t):
    for i in range (times):
       t.speed(0)
       t.undo()
       t.undo()
john.hideturtle()
# Making the Z
john.speed(0)
john.color("green")
john.begin_fill()
 
john.left(60)
john.forward(100)
john.left(120)
john.forward(100)
 
john.right(90)
john.forward(10)
john.right(90)
john.forward(120)
 
john.right(120)
john.forward(200)
john.left(120)
john.forward(100)
 
john.right(90)
john.forward(10)
john.right(90)
 
john.forward(120)
john.right(120)
john.forward(100)
 
john.end_fill()
 
# Making the circle
 
def draw_square(some_turtle):

    for i in range (1,5):
        some_turtle.forward(200)
        some_turtle.right(90)

def draw_art():
    window = turtle.Screen()
    window.bgcolor("black")
    #Turtle Brad
    brad = turtle.Turtle()
    brad.shape("turtle")
    brad.color("yellow")
    brad.speed(0)
    brad.pensize(2)
    for i in range(1,37):
        draw_square(brad)
        brad.right(10)
    undo(400, brad)
    brad.hideturtle()

    

draw_art()
  

undo(36, john)

def channel_one():
    john.fillcolor("blue")
    john.begin_fill()
    john.forward(-50)
    john.forward(100)
    john.left(120)
    john.forward(100)
    john.left(120)
    john.forward(100)
    john.left(120)
    john.forward(100)
    john.end_fill()
    john.penup()
    #getting to center of triangle (pythagorean theoream)
    john.goto(0,15)
    john.pendown()
    #writing 1
    style=('normal', 20, 'bold')
    john.pencolor('white')
    john.write('1', font=style, align='center')

    john.left(90)
    john.penup()
    john.forward(100)
    john.pencolor('black')
    style=('normal', 30, 'bold')
    john.pendown()
    #top, writing to show channel 1
    john.write('Channel', font = style, align ='center')
    john.hideturtle()
    wn.bgcolor('lavender')
    #timer
    time.sleep(3)
    #undo
    undo(42, john)
    john.speed(0)


def daily_news():
  '''shows the daily news'''
  style=('normal', 20, 'bold')
  john.write('Daily News', font=style, align='center')
  john.hideturtle()
  time.sleep(3)
  undo(3, john)
  john.penup()
  style2=('normal', 20, 'bold')
  john.home()
  john.left(90)
  john.forward(100)
  story = "Today's story is about Tom Scott, the famous British YouTuber."
  john.write(story, font=style2, align='center')
  wn.bgcolor('lightblue')
  john.hideturtle()
  john.forward(-100)
  style3=('normal', 10, 'bold')
  report = "About a month ago, YouTuber Tom Scott had an idea. He wanted to write a code, which be added to a website, ask for information, and change something based on that info. He wrote some code and managed to do this, even though it was complicated and tedious a times. In his video, the title updates, based on how many views the video has.  \n For example if the video has a million views the descriptioon will update to 1 million views. We found this pretty cool and wanted to share it with other people.  "
  john.write(report, font = style3, align = 'center')
  time.sleep(10)
  undo(43, john)
  john.speed(0)

def weather_report():
  wn.bgcolor('lightblue')
  '''does the weather'''
  style=('normal', 30, 'bold')
  john.fillcolor('navy')
  john.goto(0,0)
  john.begin_fill()
  john.forward(-50)
  for i in range(3):
    john.forward(100)
    john.left(120)
  john.end_fill()
  john.forward(50)
  john.penup()
  john.goto(0, 16)
  john.pencolor('white') #We make the second story, channel 2
  john.write('2', font=style, align='center')
  john.left(90)
  john.penup()
  john.forward(100)
  john.write('Channel', font=style, align='center')
  john.hideturtle()
  time.sleep(3)
  undo(20, john)
  john.hideturtle()
  john.penup()
  style3=('normal', 15, 'bold')
  john.home()
  john.left(90)
  john.forward(100)
  john.left(90)
  john.forward(100)
  john.left(90)
  style4=('normal', 10, 'bold')
  john.color('purple')
  john.write("Weather in Toronto", font = style4, align = 'center')
  john.forward(125)
  john.write("\n\nMostly partly cloudy\n and around 25 C (77 F)\n for the day, \nclear at night.\n Perfect temperature\n for going outside!", font=style4, align = 'center') #We tell the weather
  john.forward(-125)
  john.left(90)
  john.forward(215)
  john.right(90)
  john.color('black')
  john.write("Weather in Washington, DC, USA:", font=style4, align='center')
  john.forward(125)
  john.write("Partly cloudy \n for most of the day,\n predicted thunderstorms\n in the evening.", font=style4, align='center')
  john.forward(-70)
  john.right(90)
  john.forward(100)
  john.left(90)
  john.forward(200)
  john.write ("It's 6/25/20 and...", font=style3, align = 'center') #Tell the date
  john.forward(50)
  john.write("That's it folks!", font=style3, align = 'center')#We end with a that's it folks!
  time.sleep(8)
  undo(25,john)
  john.hideturtle()
  john.speed(0)

def tiger_jokes():
  john.penup()
  #intro
  '''Tiger Jokes'''
  john.hideturtle()
  wn.bgcolor('lightblue')
  style=('normal', 30, 'bold')
  john.fillcolor('navy')
  john.goto(0,0)
  john.begin_fill()
  john.forward(-50)
  for i in range(3):
    john.forward(100)
    john.left(120)
  john.end_fill()
  john.forward(50)
  john.penup()
  john.goto(0, 16)
  john.pencolor('white') #We make the second story, channel 2
  john.write('3', font=style, align='center')
  john.left(90)
  john.penup()
  john.forward(100)
  john.write('Channel', font=style, align='center')
  john.hideturtle()
  time.sleep(3)
  undo(20, john)
  john.pencolor('black')
  style=('normal', 20, 'underline')
  john.penup()
  john.speed(0)
  john.hideturtle()
  john.left(90)
  john.forward(100)
  john.write('Jokes with TigerEye', font=style, align='center')#make john write tiger watch with tigereye
  john.home()
  style=('normal', 30, 'bold')
  john.right(90)
  style5 = ('normal', 10, 'bold')
  style6 = ('normal', 5, 'bold')
  john.write("This is joke is built into python itself.", font = style5,align='center')
  john.forward(100)
  john.write("Go to python, open a new module, and write from __future__ import braces.", font = style5, align='center')
  john.forward(100)
  john.write("Run the program and look at which error pops up. ",font = style5, align='center')

  time.sleep(5)
  undo(20, john)
  
def COVID_19():
  #intro
   john.hideturtle()
   wn.bgcolor('lightblue')
   style=('normal', 30, 'bold')
   john.fillcolor('navy')
   john.goto(0,0)
   john.begin_fill()
   john.forward(-50)
   for i in range(3):
      john.forward(100)
      john.left(120)
   john.end_fill()
   john.forward(50)
   john.penup()
   john.goto(0, 16)
   john.pencolor('white') #We make the second story, channel 2
   john.write('4', font=style, align='center')
   john.left(90)
   john.penup()
   john.forward(100)
   john.write('Channel', font=style, align='center')
   john.hideturtle()
   time.sleep(3)
   undo(20, john)
   john.home()
   john.penup()
   john.left(90)
   john.forward(200)
   john.write("Covid-19 Stats", font = style, align = 'center')
   john.right(180)
   john.forward(80)
   john.write("Total cases: 9.44M", font = style, align = 'center')
   john.forward(80)
   john.write("Total recovered: 4.76M", font = style, align = 'center')
   john.forward(80)
   john.write("Total deaths: 483K", font = style, align = 'center')
   time.sleep(5)
   undo(30, john) 
   john.left(90)
   john.penup()
   john.forward(100)
   john.write("Total U.S. cases: 2.43M", font = style, align ='center')
   john.right(180)
   john.forward(50)
   john.write("Total U.S. recoveries: 747K", font = style, align ='center')
   john.forward(50)
   john.write("Total U.S. deaths: 124K", font = style, align ='center')
   john.forward(50)
   time.sleep(5)
   undo(20, john)
   john.left(90)
   john.penup()
   john.forward(100)
   john.write("Total Canadian cases: 102,431", font=style, align='center')
   john.right(180)
   john.forward(50)
   john.write("Total Canadian recoveries: 65,001", font=style, align='center')
   john.forward(50)
   john.write("Total Canadian Deaths: 8,484", font=style, align='center')
   time.sleep(5)
   undo(42,john)
   
def famous_birthdays():
  #intro
  john.hideturtle()
  wn.bgcolor('lightblue')
  style=('normal', 30, 'bold')
  john.fillcolor('navy')
  john.goto(0,0)
  john.begin_fill()
  john.forward(-50)
  for i in range(3):
     john.forward(100)
     john.left(120)
  john.end_fill()
  john.forward(50)
  
  john.goto(0, 16)
  john.pencolor('white') #We make the second story, channel 2
  john.write('5', font=style, align='center')
  john.left(90)
  john.penup()
  john.forward(100)
  john.write('Channel', font=style, align='center')
  john.hideturtle()
  time.sleep(3)
  undo(20, john)
  john.home()
  john.left(90)
  john.penup()
  john.forward(100)
  john.write('Famous Birthday on June 25:', font = style, align = 'center')
  john.left(180)
  john.forward(100)
  
  style2 = ('normal', 20, 'bold')
  john.write('Lele Pons', font=style, align='center')
  style3 = ('normal', 10 , 'bold')
  john.forward(100)
  
  john.write('Lele Pons, a YouTuber and Internet phenomenon.', font=style2, align='center')
  time.sleep(4)
  undo(30,john)

def story():
  import random

  print("You're in the deep blue ocean, sailing with the soft breeze.")
  print('"Where are we going?", you ask your captain.')
  print("Your captain, SparklyFlowers, replies with a simple you'll see.")
  print("Suddenly, there is a loud bang. SparklyFlowers falls down.")
  print("She swims back up and calls to you - 'jump down here and let's swim to shore!'")
  n = input("What do you do? Do you listen to her and jump down to the ocean or do you stay on the ship as SparklyFlowers swims away? Input 'listen' or 'stay'")
  if n == 'stay':
    print("You chose to stay on the ship. You abandon SparklyFlowers in the water.  Suddenly, your ship sinks really fast.  You and the rest of your crew besides SparklyFlowers fall to the ocean. You'll have to rely on your swimming skills now!")
    goodOrNot=input("How good are you at swimming? Please input 'good' or 'bad'.")
    if goodOrNot=='bad':
      print("Sorry... but you have died.")
    elif goodOrNot=='good':
      print("Endurance is important now.")
      m=random.randint(1, 2)
      if m==1:
        print("Congrats, you made it! Give yourself a pat on the back.")
      elif m==2:
        print("Sorry... you have died in the battle with endurance.  OOOOOOOF")
  elif n == 'listen':
    print("You choose to listen. You jump down to swim with SparklyFlowers. She helps you swim to shore. You then realize that the shore is on an abandoned island.  You will have to survive by yourselves until you can call for help.")
    print("As soon you reach the island, you take stock of your inventory.  SparklyFlowers has a FirstAid kit and a sword.")
    print("You also have a sword, and you also have some food and matches.  The matches seem to be drenched and not working, however.")
    print("You set off for the inside of the island with SparklyFlowers.")
    print("Suddenly, from your left, a wild boar comes charging.")
    run = str(input("Do you want to run from the boar, or attack it? Input 'attack' or 'run'."))
    if run == 'run':
      print("You run through the jungle, but the boar is too fast and you get sliced to pieces by its tusks.")
    elif run == 'attack':
      print("You and SparklyFlowers keep the boar away with your swords then slice it to pieces.  Now you have meat to eat later.")
      print("You have to find some shelter.")
      shelter = str(input('Where do you go?  To the left side of the island?  Or maybe around to the back of the island, behind the mountain?  Make sure your input is "left" or "back".'))
      if shelter == 'left':
        print('You trek through the hot jungle for a few hours with SparklyFlowers, and you finally reach your destination. When you get there, all you see it open beach close to water, and there\'s not many trees to be seen nearby.  This might not be the best place to set up camp, but it will have to do.') 
        print('To build a camp, you need trees to set up a building, but there are no trees nearby.  You reach for some driftwood, but then a shark suddenly comes out of the water and bites you hand off.  You scream in pain, and SparklyFlowers use her FirstAid Kit.  It\'s not enough, and you bleed to death.')
      elif shelter == 'back':
        print('You trek for 5 hours through the hot jungle to get to the other side of the island.  There you find that the mountain gives you some shade from the bright sun, and there are trees and other plants in abundance, meaning food.')
        print('You and SparklyFlowers move through the forest, gathering wood and supplies.' + '\n')
        print('After a few hours, the camp is finished.  There is a fire up and roaring in the middle, and the boar from earlier is being sizzled over it.  You have a small building with four walls, above the ground, that you will sleep in.  There is another building next to it, that is your workplace.  There you will craft tools.')
        print('The boar looks delicious.  You take it off the fire.  You and SparklyFlowers begin to eat the boar.  It is delicious after a long day of hard work.')
        print('\n' + 'After telling stories by the fire, it is time to go to bed. It is getting late and you should be sleepy now.  As you drift off into the wonderful dream of escaping this island, you hear a sudden growl.  You disregard it as nothing important, maybe just your stomach growling, but then you realize that your stomach is full and neither you or SparklyFlowers has a reason to growl.  You jump up and hear more growling coming from outside the house.  You wake SparklyFlowers up.  "Hey what\'s going on?" SparklyFlowers asks.  Then she goes pale as she hears the growling.  "Those must be hyenas," she remarks.')
        print('The hyenas are hungry.  They can smell you on the inside.  One breaks through the wood door and come running.  You slash its head off with your sword.')
        hyena = str(input('Will you fight or flee?  Make sure to input "fight" or "flee"'))
        if hyena == 'flee':
          print('You decide to jump out of the building.  You not surprisingly land in a hyena\'s jaws, where it tears you to pieces.  Don\'t think about it too much.')
        elif hyena == 'fight':
          print('You decide to fight the hyenas off.  Then you have a great idea. You grab a piece of firewood and you light it up.  SparklyFlowers does the same.  The hyenas see the fire and get scared and run.  You sigh with relief.')
          print('As you drift back to sleep, you dream of eating hyenas...')
          print('The next day, when you wake up, the sun is burning hot, but since you chose to camp behind the mountain, it doesn\'t scorch you.  You walk outside, and find SparklyFlowers preparing some fruit from the forest to eat.  SparklyFlowers gives you the bigger half of the fruit.  You are glad that you have such a generous captain.')
          print('You need to find another food source other than just fruits.  You try fishing.')
          print('At first, you try just grabbing the fish with your hands.  Obviously, it doesn\'t work as the fish are too fast.  Then, you try using a sharp stick.')
          print('You will need to go underwater, because the water seems to bend the light.')
          print('At last, you catch your first fish.  You take it back to your camp.  SparklyFlowers gets a fire going, and you grill the fish and eat it for lunch.')
          print('It is delicious.')
          print('You then explore the island and find some meat for dinner.')
          print('Three decades pass by like this, with no one coming by to help you and SparklyFlowers.')
          print(':(')
          print('At last, you see a ship come by.  You wave and it comes over.  The captain of the ship says, "Hey, aren\'t you the people that went missing for a few decades?"')
          print('You and SparklyFlowers are gladly rescued and given a welcome parade when you arrive back on the mainland.')
          print('But, one night, as you are sleeping in your bed, you have a dream.  You are back on the island with SparklyFlowers, and the mountain that you lodged behind starts erupting.')
          print('You wake up and scream, only to find that you are still on the island, and it was all a dream.')
          print('Then, just like in your dream, the earth starts shaking and hot lava starts spewing out of the top.')
          volcano = input('Do you run to the sea, or do you run towards the other side of the island, or do you run up the volcano?  Make sure that your answer is "sea", "other side", or "volcano".')
          if volcano == 'volcano':
            print('What are you trying to do die and get scalded')
          elif volcano == 'other side':
            print('You run to the other side, only to find that it is also covered in lava.')
            print('ded')
          elif volcano == 'sea':
            print('You run into the sea and as the lava comes rushing towards you, it slowly hardens.  It destroys your camp, but all that really matters is that you are still alive.')
            print('In a few days, scientists come and rescue you.  They felt the rumbling of the volcano from so far away.  They picked up seismic waves and detected that it came from your island.  They find you, and this time you are actually saved.')
            print('Congratulations, you have beat the game!')
  undo(5, john)
  
channel = input("What channel do you want to watch? Please input 1, 2, 3, 4, or 5. If you would like to watch all the channels, please input anything else. ")
if channel=='1':
  channel_one()
  daily_news()
elif channel == '2':
  weather_report()
elif channel == '3':
  tiger_jokes()
elif channel=='4':
  COVID_19()
elif channel=='5':
  famous_birthdays()
elif channel=='6':
  story()

else:
  channel_one()
  daily_news()
  weather_report()
  tiger_jokes()
  COVID_19()
  famous_birthdays()
  story()

# Credits
john.penup()
john.hideturtle()
style=('normal', 20, 'underline')
john.home()
john.left(90)
john.forward(50)
john.color('black')
john.write("Credits", font = style, align = 'center')#And here are the credits
john.forward(100)
style7=('normal', 20, 'bold')
wn.bgcolor('lightgreen')
john.write("ZANDERMAN NEWS",font = style7, align = 'center')
john.right(180)
john.forward(150)
john.write("SparklyFlowers",font = style7, align = 'center')#SparklyFlowers
john.forward(50)
john.write('TigerEye123', font = style7, align = 'center')#TigerEye123
john.forward(50)
john.write("Zanderman", font = style7, align = 'center')#And Zanderman
john.forward(50)
john.write("BlueJay43", font=style7, align='center')
time.sleep(3)
undo(13,john)
john.speed(0)
john.home()
john.right(90)
style=('normal', 20, 'bold')
john.write("Thanks For Watching!", font = style, align = 'center')



wn.mainloop()
