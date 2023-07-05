#The Project has five components - Header.astro, Home.astro, About.astro, services.astro, contact.astro

#Inside the "header Component" the responsive navbar is created with interactive "hamburger menu" which uses 
addeventlistner method while clicking the toggle is changed based on the active class.

#In services section there is an "interactive carousel" which has two buttons "prev-button and next-button". 

#To easily access the buttons and parent divisions javascript dataset is used so it won't be confused with class attributes
#when the button is clicked, if the dataset attribute is "next" and the condition is 1 then it will go to the next slide same for previous if it is -1 then goes to the slide before by using the ternary operation.

#To access the slides, from button attribute we are getting the closest parent which is the data-carousel and from the parent we are accessing the data-slides attribute.

#Then converting the slides to the array from children class. And getting the index of the active class which is first slide.

#By using the index of the active class we can check:
  -if the index is less then 0. we go backwords from first image which is the last image
  -if the index length is greater than the length of the children class array. we go past our last slide we start the index from first
  
#for each slide change we set the active attribute for the current slide and remove it after the slide changes. 