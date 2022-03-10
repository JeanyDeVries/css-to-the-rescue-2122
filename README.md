# CSS to the Rescue ~ DJ Control Panel

# Table of contents
[Result](#Result)  
[Concept](#Concept)  
[Week 1 ~ Making the concept](#Week1)  
[Week 2 ~ Styling the page](#Week2)  
[Week 3 ~ Adding the interactions](#Week3)  
[ Week 4 ~ Last changes](#Week4)

# Result  <a name="Result">

# Concept <a name="Concept">
The concept is to make a interactivee DJ control panel which interacts with the crowd. The interactions are handled by buttons and sliders. 
Interaction ideas:
- Crowd that dances upwards
- Light brighten up
- Set music louder with a slider (sounds a slider are both made with javascript)
- Discoballs moves or lightens up
- Off switch
- Maybe move the circle pads
- Add some fun sounds to some buttons

I also want to implement some small details if I have the time.
Detail ideas:
- Cursor is a headset or some other icon


# Week 1 ~ Making the concept  <a name="Week1">
To start with the end project I first decided I wanted to work with a interactive control panel. I chose this because I thought this would be nice in combination with my game development, plus you had a lot of freedom on what to make. 
The second thing for me to do was sketching. I needed to have an idea on what I wanted to make. So I thought of different ideas and drew them out, see pictures below. 

!<img src="https://user-images.githubusercontent.com/44086608/154667193-96b281ac-8ed6-412b-ba8a-4073e3e138e4.jpg" width="400" height="300"> !<img src="https://user-images.githubusercontent.com/44086608/154667192-15966f4e-a052-484f-8645-43afebe49e3f.jpg" width="400" height="300">

I chose my first idea of the DJ control panel. The reason why is because the control panel is easy to implement because a dj already has one. Plus you can have so much interactions with it. 
 
# Week 2 ~ Styling the page  <a name="Week2">
My focus for this week was to create the scene without any interactions first. I wanted to start with the styling and see how it would turn out. 
The result was this at the end of the week:

https://user-images.githubusercontent.com/44086608/154668674-b66bdfa5-eb13-4d03-b484-77360bf2e13f.mp4

I'm happy with how it looks, but sadly it isn't responsive yet. I found out that my weakness in CSS lays with creating the layout and making it responsive. 

The things that I struggled with is as I said making it responsive. I got a tip from a teacher to use grid instead of flex for the dj panel so that it alligns the empty spaces according to the screen size.

https://user-images.githubusercontent.com/44086608/155135470-770b56dc-be58-468a-8f85-e8b8d573a1f4.mp4

The second thing I struggled with was the on click with my buttons. For some reason if I clicked the button, the others would move as well, see video below. After a while I finally knew what was happening. It is a flex so if one button moves down the buttons below it move as well. 

https://user-images.githubusercontent.com/44086608/155136853-e3752ee8-e735-43ff-9dcf-5c6d8b3523fa.mp4

# Week 3 ~ Adding the interactions <a name="Week3">
As you saw in week 2 I still hadn't made the site responsive and as this is a course of CSS it is an important case to have it working. The first step I had to do was change from flex to grid. This way it would scale nicely together. After that has been done, it still wasn't perfect. After fooling around I found out that using the calc function was the best way to make it work. I used the view width in this case. It's still not perfect, but for me who has a little knowledge of CSS makes me already a bit happy with the result. It does need some tweaking off course, but I don't know if I'll have time for it. 

https://user-images.githubusercontent.com/44086608/156917795-22de7d6f-7a3a-46e5-aa21-e084dfc940dd.mp4

The second thing that did not work the way I wanted was the interactions. I made a big mistake using list items for the interactions. I thought it would be possible with the active state from the list item. But it made it a lot more complicated then I wanted. The thing that made it difficult was selectors. I wanted to select the item that I wanted to change as well, but it would be a whole spaghetti code for me. I looked at someoone else his project and saw them using labels and inputs. This was a lot more cleaner with the css. You only had to check if the label with the correct input is checked and then I could add the element I wanted to change as well. It was a bit time eating to change mu whole code around, because some of the scaling didn't work. It didn't work because I added the main to the body. But I'm happy that it works, and I learned that I need to think beforehand doing these things. 

From the feedback I got this week, was to have a reference for the control panel. So I looked at some pictures online and I found one that I liked: 

### Reference
![image](https://user-images.githubusercontent.com/44086608/156918028-5b5b012b-f1f1-402a-acac-c5fb7fc2156d.png)

I then changed the looks of my control panel and I think it already looks a lot better than before: 
![image](https://user-images.githubusercontent.com/44086608/156918058-755cf2ca-435b-4e30-80c1-1cb56a533551.png)

At last the fun part of this week. Adding the interactions. I wanted to add to the party ambiance. I created confetti, disco ball stretching and people jumping more up and down. As I told you before I looked if the input was checked and if so I added the parent element to it, see code below. This way I could change properties from the elements. If I wanted to change the variables, I could just grab the main element. 

Changing a variable
```
    input:nth-child(2):checked ~ main{
        --spinningSpeed: 1s;
    }
```

Changing a element
```
    input:nth-child(5):checked ~ main li:nth-child(3) label:nth-child(5){
        box-shadow: 0 0 0  transparent,
                    0 0 0  transparent,
                    inset 0 0 10px #2e2e2e;        
        margin-top: 4px;
    }
```

# Week 4 ~ Last changes <a name="Week4">
 This week I added a 2 more interactions, discoball lighting and disco lights. I then gave each button a interaction, which is sadly just the interactions I already had. But within this time it was a bit difficult for me to make 16 interactions, so I stuck with 7. 
I was also not happy with how responsive the site was with the control panel. I made a start, but it was not perfect. So after retweaking some code I finally had the result I wanted: 

https://user-images.githubusercontent.com/44086608/157633437-6d3e2017-c679-4a72-ac18-17b80c5e26d3.mp4

