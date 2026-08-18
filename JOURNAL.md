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


# 16/08/2026 

It became a update journal rather than normal continuous journal. 

First of all, I dumbed my thoughts of doing first charge. It will be no longer a feature. Just a general USB hub to get it started. 

My upstream port is a male connector so that I don't have to use extra cable. And the downstream ports are all vertically positioned. Trying to shrink the size as much as I can.  

**Note to reviewers**

First of all, I thought to make it a 2 layer board. But USB3 is such a high speed connection that it is not recommended to use a 2 layer board cause it needs a reference plane. So It is a 4 layer board.  

Now, there is nothing left to update without finishing the routing focusing on routing -_-

<img width="726" height="373" alt="image" src="https://github.com/user-attachments/assets/581e7195-3ac3-42aa-9c04-209a3165e5b4" />

<img width="794" height="401" alt="image" src="https://github.com/user-attachments/assets/636ea2b2-b845-413a-9878-9e02566ba42c" />

# 17/08/2026

Routing update ! it is turning out pretty good. I like it 

<img width="832" height="629" alt="image" src="https://github.com/user-attachments/assets/ee8532d1-9399-48f7-b676-8cfe2aaaebfa" />

# 18/08/2026 

Finished the routing. There is nothing to journal about it but I can write about the thought process. 

The board is a 4 layer board. First layer is  signal layer with all of the differential pair. And the 2nd layer is GND plane which is a reference plane for the differential pair. 

3rd layer is a power plane. There is  1.2V, 3V3 and 5V 

4th layer is for decoupling caps and extra IO signal routing. 

Finally the board is finished on routing. 

### Why no case for my hub 

there is lot of free space. I will use standoff. But not for the bottom part otherwise it will increase the height and I will not be able use with my laptop cause the upstream port is Male connector. So only top case i can make but still I have vertical USB port so I don't think a top case would be suitable 

<img width="821" height="579" alt="image" src="https://github.com/user-attachments/assets/412bea27-ece8-4770-a265-287dac7f2982" />

<img width="839" height="602" alt="image" src="https://github.com/user-attachments/assets/8ac9025f-550a-4a54-82d5-c3e9b081f778" />

<img width="801" height="482" alt="image" src="https://github.com/user-attachments/assets/09aa1e16-1da5-43b9-9d23-f812ff7ff79a" />


