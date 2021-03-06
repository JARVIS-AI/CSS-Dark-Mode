# How to Use
Custom Stylesheets can be applied using CSS Injection within your browser. The easiest method to do this is to use the browser extension called "Stylus". Download links can be found below:

[Stylus Extension](https://github.com/openstyles/stylus)

# Screenshots

![Google](https://github.com/PINPAL/CSS-Dark-Mode/raw/master/README/Google.png) 
![Google](https://github.com/PINPAL/CSS-Dark-Mode/raw/master/README/Google2.png)
![Stylus](https://github.com/PINPAL/CSS-Dark-Mode/raw/master/README/Stylus.png) 
![TypingClub](https://github.com/PINPAL/CSS-Dark-Mode/raw/master/README/Typing.png)
![TypingClub](https://github.com/PINPAL/CSS-Dark-Mode/raw/master/README/Typing2.png)
![iCloud Photos](https://github.com/PINPAL/CSS-Dark-Mode/raw/master/README/iCloud.png) 

# Progress List

99% - TypingClub

95% - iCloud Photos

80% - Stylus IDE 

70% - Google 

40% - Amazon

0% - GitHub

# To-Do List
## Google Dark Mode
 - [x] Flights  - "fly from la to nyc"
 - [x] Hotel Booking "park inn cologne"
 - [ ] Minor Stuff "p.f. chang's"
 - [x] Sidebar Twitter "new york"
 - [x] Make Bubble Buttons Pop
 - [ ] Brighten Star Ratings "park inn cologne"
 - [x] The entire News section
 - [x] The navbar on Finance section
 - [x] Boxes in boxes in personal section
 - [ ] "More" drop down
 - [ ] "Settings" drop down
 - [ ] "Safe Search" drop down
 - [ ] App Drawer (top right)
 - [x] Preview Tables
 - [ ] Fix hover mini navbar to reveal lower navbar
 - [x] Weather
 - [ ] Google images upload
 - [ ] Google top left nav logo in Images/News etc
 - [ ] League Tables "g2"
 - [ ] Overlapping bottom bar "entombed"
 - [ ] "More Images" on sidebar "entombed"
 - [ ] Hex color picker
 - [ ] Quick translate buttons / dropdowns
 - [ ] Fix a billion more bugs

# Design Guidelines
## Basic Design Language
The basic design language focuses on a dark interface with a touch of color and motion to signify buttons and actions when pressed or hovered.
The most basic background color should have a hex value of:
```
#292C30
```
White text will be used primarily however using text with an RGBA value can also be used in order to create darker text. In this format you can vary the alpha value in order to get the desired gray. For example, an element which should not be the main focus of the user could have a alpha of 50% eg:
```cs
  rgba(255,255,255,0.5)
```
Links should be used a light blue color with the following hex value. The hover effect can be created by applying a 50% alpha.
```
#2a90fc
```

## Big Box
This one is used in order to hold content. Don't use it too much. Large titles should be placed outside the box.
```css
{
  background: #2F3439;
  box-shadow: 5px 5px 10px rgba(0, 0, 0, 0.25);
  text-align: left;
  color: white;
  border-radius: 25px;
  padding: 15px;
  line-height: 1.6;
  border-style: solid;
  border-color: rgba(255, 255, 255, 0.03);
  border-width: 2px;
}
```

## Buttons
This is a button, the rest is pretty self-explanatory. Links are NOT equal to buttons. Use wisely!
```css
{
  background: linear-gradient(to right, #55B49D , #2B7DCA);
  box-shadow: 5px 5px 10px rgba(0, 0, 0, 0.1);
  text-align: center;
  border-radius: 25px;
  padding-top: 5px;
  padding-bottom: 5px;
  padding-left: 25px;
  padding-right: 25px;
  color:white;
  font-size: 18px;
  border: none;
  font-weight: normal;
  text-transform: capitalize;
  outline: none;
}
```
Don't forget a fancy hover effect!
```css
:hover {
  filter: hue-rotate(90deg);
}
```

## Search Boxes
These can also be used for drop-downs or checkboxes.
```css
{
  background: rgba(200, 200, 255, 0.2) ;
  box-shadow: 5px 5px 10px rgba(0, 0, 0, 0.1);
  text-align: left;
  border-radius: 25px;
  padding-top: 5px;
  padding-bottom: 5px;
  padding-left: 25px;
  padding-right: 25px;
  color:white;
  font-size: 18px;
  border-style: solid;
  border-color: rgba(255, 255, 255, 0.05);
  border-width: 2px;
  outline: none;
}
```
Again, don't forget the hover effect!
```css
:hover {
  background: linear-gradient(to right, rgba(149,136,213,0.4) , rgba(171,89,147,0.4));
}
```

## Scroll Bars
Title says it all. If neccesary here is the code for a custom scrollbar. The classes may need to be changed for a specific element.
```css
::-webkit-scrollbar {
  width: 9px;
  height: 9px;
}
::-webkit-scrollbar-track {
  background: rgba(255,255,255,0.08);
  border-radius: 10px;
}
::-webkit-scrollbar-thumb {
   background: rgba(255,255,255,0.20);
   border-radius: 10px;
}
::-webkit-scrollbar-thumb:hover {
   background: rgba(255,255,255,0.25);;
}
```
