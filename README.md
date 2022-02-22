# CSS to the Rescue ~ DJ Control Panel

# Concept
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


# Week 1 ~ Making the concept
To start with the end project I first decided I wanted to work with a interactive control panel. I chose this because I thought this would be nice in combination with my game development, plus you had a lot of freedom on what to make. 
The second thing for me to do was sketching. I needed to have an idea on what I wanted to make. So I thought of different ideas and drew them out, see pictures below. 

!<img src="https://user-images.githubusercontent.com/44086608/154667193-96b281ac-8ed6-412b-ba8a-4073e3e138e4.jpg" width="400" height="300"> !<img src="https://user-images.githubusercontent.com/44086608/154667192-15966f4e-a052-484f-8645-43afebe49e3f.jpg" width="400" height="300">

I chose my first idea of the DJ control panel. The reason why is because the control panel is easy to implement because a dj already has one. Plus you can have so much interactions with it. 

# Week 2 ~ Styling the page
My focus for this week was to create the scene without any interactions first. I wanted to start with the styling and see how it would turn out. 
The result was this at the end of the week:

https://user-images.githubusercontent.com/44086608/154668674-b66bdfa5-eb13-4d03-b484-77360bf2e13f.mp4

I'm happy with how it looks, but sadly it isn't responsive yet. I found out that my weakness in CSS lays with creating the layout and making it responsive. 

The things that I struggled with is as I said making it responsive. I got a tip from a teacher to use grid instead of flex for the dj panel so that it alligns the empty spaces according to the screen size.

https://user-images.githubusercontent.com/44086608/155135470-770b56dc-be58-468a-8f85-e8b8d573a1f4.mp4

The second thing I struggled with was the on click with my buttons. For some reason if I clicked the button, the others would move as well, see video below. After a while I finally knew what was happening. It is a flex so if one button moves down the buttons below it move as well. 

https://user-images.githubusercontent.com/44086608/155136853-e3752ee8-e735-43ff-9dcf-5c6d8b3523fa.mp4


