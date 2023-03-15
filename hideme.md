so for this one just download the file provided in the challenge it's a picture(image)
next up if you try to open it with your regular images viewer you wouldn'tsee much , just the logo of picoCTF
so what i did next was to exiftool it --> it didn't work everythig was normal.
next up i did think about binwalk and so i did 
![image](https://user-images.githubusercontent.com/76063719/225462600-4d1ceeb7-2a68-464c-b009-16841607c58b.png)

as you can see we actually have some hidden files in there 
extract them using "**binwalk -e flag.png**"
we get a file and inside it there is another file called secret , interesting 


![image](https://user-images.githubusercontent.com/76063719/225463156-7e52af57-90f1-4d7c-be5b-7eaf1add2504.png)



so after we pop into the secret folder we will find another image called the same thing as the one we started with **flag.png**
this time viewing this image reveals the actuall flag.

![image](https://user-images.githubusercontent.com/76063719/225463983-595eead8-d66b-461d-8daf-9a6230db202d.png)


 so there's the flag congrats 
 
 
 final thoughts : i probably should look for a tool that scans images and gets the text in them , i've already heared john hammond talks about something like that, 
 anyway for now let's just submit our flag
 
 **picoCTF{Hiddinng_An_imag3_within_@n_ima9e_683e597b}**
