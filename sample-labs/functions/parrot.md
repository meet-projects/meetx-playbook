

## Polly Wants a Cracker?

![parrot](http://1.bp.blogspot.com/-HDI-XiLird8/ToaJsehSY0I/AAAAAAAABso/XHXOU_qDK3k/s1600/Parrot+Funny+Pictures_1.jpg)

In this lab you'll be training some parrots with special talents and get some practice creating your own methods. 

Parrots love to mimic their human companions. In this lab you'll give your parrot methods a word or phrase as an argument and your parrot will take your argument, do something to it, and say then it back to you in their own quirky way. Read on for some of the key concepts you'll need to use to complete this lab.

###Method Arguments

We define methods with arguments as a way of to give our methods an extra piece of information or data to work with. An argument can be any of the data types When you're defining a method the arguments are just placeholders that represent what you'll pass in when you call your method. 

```
def my_method_name(argument)
  argument.upcase
end

puts my_method_name("In this example my argument is a string!")
```

In the example above I would see this printed to my terminal: IN THIS EXAMPLE MY ARGUMENT IS A STRING!

We can also save arguments to a variable and pass that in to our method call. The example below will have the same result as the example above. 

```
def my_method_name(argument)
  argument.upcase
end

sentence = "In this example my argument is a string!"
puts my_method_name(sentence)

```

###Return Values

A method's return value is always the last line of code before the "end" keyword. This is important to keep in mind if you're using puts inside of your method. If you use puts inside your method what you see printed to the screen may be different than your return value. You may sometimes see the last line with a "return" keyword in front of it, but it's not necessary to include this. In Ruby the last line is always the return value whether or not you write out the word "return". 

```
  def say_pet_name(pet_name)
    puts "My pet's name is #{pet_name}"
    "My pet's name is Ralph"
  end

  puts say_pet_name("Coco")

```

If you run the above example you'll actually see two lines printed to the screen. 

My pet's name is Coco
My pet's name is Ralph

The puts inside of the method is printing the line with the pet_name argument string interpolated, while the second line is the result of puts-ing the return value of the say_pet_name method. 

###Method Chaining

You can call multiple methods on a number or string by just adding another .method onto the end. We call this method chaining. When you chain on methods they change the thing they're called on one at a time from left to right. That means that the second chained method is actually changing the return value of the method that comes before it. 

 ```
 puts "matz is my homeboy".capitalize.reverse
 puts "matz is my homeboy".reverse.capitalize
 ```
If you run these two lines of code you'll see two lines printed to the screen: 
```
yobemoh ym si ztaM
Yobemoh ym si ztam
```
You can quickly see that the two lines to not create the same output. This is just one more reason why it's so important to keep track of the return values of your methods.

Okay, refresher over!

Fork and clone this lab and follow along and write your code in the `parrot.rb` file. All of the instructions for this lab are within the `parrot.rb` file. Try running your program when you are done. 


## Resources
* [Learn to Program](http://books.flatironschool.com/books/43?page=72) - [9.1 Method Parameters](http://books.flatironschool.com/books/43?page=72), page 72


## Challenges!
1.  Happy Parrot - This parrot is so happy. It accepts a 'thing' as its argument and then returns a string where it says how happy it is about the thing!
def happy_parrot(thing)
  "I am so happy about #{thing}!"
end

2. Boring Parrot - Write a method for a boring parrot that just returns whatever string you give him as an argument.1. Math Parrot - Create a method that accepts two numbers as arguments and adds them together! 



3. Friendly Parrot - This parrot greets people by returning their name and age (don't forget to pass that information in as arguments).



4. Favorites Parrot - Tell this parrot about your three favorite things and he will return "I love <that thing> too!" for each of them.



5.  Now try calling your methods below with any arguments of your choice and puts them to the screen. Like this:
puts happy_parrot("waffles")



6.  Now let's pretend you are a wizard and you want to place a spell on each of the parrots so that they speak backwards. How would you do that?




6. The spell has been broken and everyone is speaking normally again. The parrots are really excited about it though - make them shout in all caps.



