# Stable-Arcade-
An AI powered Game Dev Studio





Summary
Game development is a complex and time-consuming process that involves many time-intensive steps. The industry also has a very high barrier to entry, because as a newbie, people have to learn many complex tools, and the learning curve is difficult for most people, especially people from non-technical backgrounds. So, even though they may have good ideas for video games, they can't bring them to reality. This project demonstrates how AI can help us mitigate these challenges, and how AI is the future of Game Development.






Story
The primary idea for this project was to create an AI-powered Game Dev Studio, where AI agents play the roles of different people involved in the creation of Video Games, and they can collaboratively work on a game idea provided to them. But the scope was too big. And the next problem was that my GPU board got stuck in customs for more than 2 months. So I pivoted my idea. Instead of using AI Agents, I focused on utilizing Image Generation models like Stable diffusion to customize the game according to the user’s interest. To narrow down the scope, I choose Arcade-style Fighting Games for my project.



Enter Mugen Engine.

While looking for a way where I can build a fighting game and customize games, I remembered an old DragonBall Z game that I used to play in childhood. It was a 2D fighting game with fast-paced fighting mechanics, like Mortal Komat or Tekken. I remembered that it was built using a MUGEN Engine. I thought it might work. So I did a little research on the MUGEN Engine. After some preliminary research, I was sure that I can use the MUGEN engine to complete my project. 

Not So Fast. 

So, in my mind, there were following steps for my project : 

Use stable diffusion to create a character image from a prompt.
Use ControlNet to create images in different fight poses, like punching, kicking, etc.
Use these images to generate a MUGEN Character.
Add this character to the MUGEN Engine and play!

But when I went to implement these steps, the most challenging part was the 3rd point. 
My idea was since MUGEN characters are created using some textual values for parameters, it should be very easy to automate those steps through a Python script, which can use the generated images to create those character files. But when I went to implement it, I came to know that there are many intricacies in creating character files using a single Python script. The second challenge was that the generated images needed to be converted into a specific color palette for them to work with MUGEN. And I need to find tools and libraries in Python to resolve these issues. 

Back to Work.

After spending countless hours on the Internet, discussing with ChatGPT, and going through MUGEN documentation again and again, I finally created a combination of unique solutions, which I don’t think anyone would find online, or even generate with the help of ChatGPT. (Really proud of figuring out this part)

Now, I had a script, which I can run on a bunch of images, and in a second, I got a character that was working in MUGEN Engine, by default. 


Generated Character files for MUGEN

So now, you can create a custom character, which you can use to fight against any character you can imagine. The only limit is your imagination. 



Character select screen with created character

Git repo : 

Next steps:

The next steps in this project are the following : 

Using Automatic 1111 and ControlNet API to automate the image generation for character, and add this part to the python script, so the whole process is completely automated.
Create a custom stable diffusion model to generate MUGEN characters, so that we get the best results while creating a character.
Create a Nice User Interface so that it is easy, even for non-technical users.

Thanks a lot for this opportunity AMD. I hope I am able to bring more of my ideas to life, powered by AMD Radeon W7900 Pro. 









Automatic 1111 : https://github.com/AUTOMATIC1111/stable-diffusion-webui
Stable Diffusion Checkpoint : https://civitai.com/models/46422/juggernaut

2D Pixelart LORA : https://civitai.com/models/165876/2d-pixel-toolkit-2d
Pixelart Checkpoint : https://civitai.com/models/129879/dreamshaper-pixelart
