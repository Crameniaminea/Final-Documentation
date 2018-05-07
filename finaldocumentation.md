Corbin Osman

Guy Verrier

ETR 164

4/23/2018

Final Project Documentation

For this project, my goal was to set up an Amazon Echo using a Raspberry Pi. My final goal was to have the Raspberry Pi respond to simple phrases that I asked it.

My project outline and objectives are as follows. I first created an Amazon Developer Account which would be used to connect with the Alexa Developer Kit. This kit would be used on the Raspberry Pi as the source for the Amazon Echo. Next, after installing Raspbian on an SD card, I installed both Git and AlexaPi on the device. This allowed me to setup an installation script and create certain settings such as the operating system and device prompts. Finally, I had to connect my Amazon Developer Account to the AlexaPi service in order to run the Amazon Echo.

The first step I took for this project was purchasing the required parts and pieces. I wanted to buy these as early as I could so I had time to work on the whole project. Listed below are all the necessary parts that I obtained.

-	Raspberry Pi (I used model 3)

-	A Monitor

-	An HDMI cable

-	Keyboard and Mouse

-	MicroSD Card

-	USB Microphone

-	USB Speakers

Once I had purchased all the parts that I needed, I set to work on my first project step, which was setting up an Amazon Developer Account. I did this through the Alexa Voice Service, which allowed me to then set up my Amazon Echo. Starting off the echo creation process, I first had to fill out some basic product information, namely the product name and ID. I then set up some security settings and obtained a security profile ID which would be used to connect to my Raspberry Pi. I also obtained a client ID and a client secret for added security and connection to my Pi device.

![image of code](https://github.com/Crameniaminea/Final-Documentation/blob/master/security.png)

The next step was to create an origin and return URL to login to my Amazon Alexa Service. In order to connect my Pi device with this service I had to use the Raspberry Pi’s IP address. As a fail-safe incase the IP address did not work, I also allowed the local host access to login as well. This was the last step on the Amazon Developer Account side, so I moved over to the Raspberry Pi once I finished.

The second step for this project was to install the custom OS that I just created. To do this I needed to install Git and the AlexaPi service, or in my case, EchoPi. After connecting to the internet, I made sure my Pi device was up to date by running “sudo apt-get install update.” Once that was finished, I installed Git with the command “sudo apt-get install git.”

With Git successfully installed, I travelled to the opt folder with “cd /opt.” The next command to run is cloning the AlexaPi GitHub repository. This was done with “sudo git clone https://github.com/alexa-pi/AlexaPi.git.” With all the necessary files installed, I ran the AlexaPi setup script with the command “sudo ./AlexaPi/src/scripts/setup.sh.”

![image of code](https://github.com/Crameniaminea/Final-Documentation/blob/master/install.png)
	
This setup script will ask a bunch of installation questions. The first asks what OS is running, and I hit enter to use the designated OS. Next, it asks what device is being used, so I entered raspberrypi to let it know that the files are being installed on a Raspberry Pi device. The next few questions it asks all relate to the Amazon Developer Account that was created earlier, so I entered all the security information into the setup file. The device then proceeded to install all of the necessary files, which took roughly ten minutes.

Once this installation was finished, I configured some audio settings to enable the microphone and speakers I had set up. After that was done, I rebooted the device to finish some final installation steps. Upon reboot, I was greeted with a verbal “Hello.” This was from Alexa, so I knew the service was running upon startup. I then proceeded to ask Alexa some questions that she could respond to. Listed below are a few of the many things I asked.

-	Alexa, what is today’s date?

-	Alexa, can you beatbox?

-	Alexa, what is the weight of the sun in kilograms?

-	Alexa, why did the chicken cross the road?

-	Alexa, tell me a joke.

-	Alexa, how do I get rid of a body?

-	Alexa, who you gonna call?

-	Alexa, what is your quest?

![image of code](https://github.com/Crameniaminea/Final-Documentation/blob/master/status.png)

In reflection, I really enjoyed working on this project for class. There were a few hiccups along the journey, but all of them were easy fixes.  The biggest problem was working around the sound output. At first, I couldn’t get any sound to come from the system, and I realized that the monitor I was using didn’t have any internal speakers. After moving over to a television screen, and the sound continued to not work, I found out that I had to turn up the audio intake on my microphone. Once I had finished that, I was able to communicate to the device and receive a reply.

I loved working on this project and on something that I could use outside of school. Having this Amazon Echo will be an awesome addition to my home, being able to play music and check the current time without having to move from my seat. I will also show some of my friends how to make this device, and I know that they will love it just as much as I do.
