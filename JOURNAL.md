# 09/08/2026

Start of the project. First question : Why this project?

=> Recently I attended a hackathon in Singapore. I found out that my laptop has only two USB ports and only one of them is USB 3.0 / I had so many hardware to connect but I didn't have enough ports. 

So to remove my future inconvenience, I decided to make USB hub. As of now, I am thinking of getting started with default design (4 Downstream) 

Cheap selection is huge as well as confusing. Found a good a project in Easyeda but the main hub seems to be market out. So working with an alternative > RTS5411S-GT. 

This chip is used in Nvidia Jetson Nano board. So, it is quite good + overkilled. But I couldn't a find a reference schematics for this specific chip. 

As a result, I am cross referencing two datasheets. 

<img width="1599" height="851" alt="image" src="https://github.com/user-attachments/assets/c2905804-ff24-4734-b7c2-b69715e3731f" />

<img width="1599" height="850" alt="image" src="https://github.com/user-attachments/assets/0492f8d4-61ae-4823-b255-115346c44f53" />

# 14/08/2026 

Take a look at what I have been working on. Honestly, I don't get the motivation that I used to have I don't know why. Post Arcana Depression 

<img width="881" height="611" alt="image" src="https://github.com/user-attachments/assets/b9157e18-6657-4ac3-92c2-dc67fbc891b8" />


Honestly, past few day I am working on it bit by bit but I am now genuinely confused. What to implement now!! I had a thought for making a general USB hub but now I have to look into power delivery stuff. 

Do I need power for my downstream ports? => Yes. But the laptop 5V won't be enough to supply the 4 downstream ports. It can manage the HUB chip itself. That is the most I believe and also if I connect my phone. I definitely want it to be fast charged crazy. 

Couple of thoughts came to my mind => 
