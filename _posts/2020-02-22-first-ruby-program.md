---
title: My First Ruby Program
categories:
- projects
layout: post
---

The other day I wrote my first Ruby program, after finishing [this tutorial](https://ruby.github.io/TryRuby/).

The computer asks for a yes or no response, then displays one of my wife's unpublished poems. At the end, I put in an Easter egg for my wife with an additional yes or no question. <span>&#128578;</span>

Here's the whole program:
```ruby
def woodford_reserve
  puts " ________________________________________________"
  puts "\|                                                |"
  puts "\| \"Woodford Reserve\"                             |"
  puts "\|  by Jane Clark Scharl                          |"
  puts "\| ---                                            |"
  puts "\| Before this, I’ve never seen my dad            |"
  puts "\| drink bourbon. Now, he slightly tips his head, |"
  puts "\| rolls liquor on his tongue, and says exactly   |"
  puts "\| what a bourbon-drinker would: perfectly        |"
  puts "\| balanced depth, slight smoke, a lingering glow |"
  puts "\| all evocative of things that I don’t know.     |"
  puts "\|________________________________________________|"
end
puts "Would you like to read the poem? (y/n)"
permission = gets.chomp()
if permission == "y"
  puts "\nGreat! Here it is:"
  sleep(1.5)
  puts woodford_reserve
  sleep(3)
  puts "Psst...Do you want to know a secret? (y/n)"
  secret_permission = gets.chomp()
  if secret_permission == "y"
    puts "\n<3<3<3<3<3<3<3<3<3<3<3<3<3"
    puts "<3                      <3"
    puts "<3  SCOTTY LOVES JANE   <3"
    puts "<3                      <3"
    puts "<3<3<3<3<3<3<3<3<3<3<3<3<3\n"
  else
    puts "Ok, sounds like you don't want to know."
  end
else
  puts "Fine. Suit Yourself."
end
```
