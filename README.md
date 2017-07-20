## Inspiration

Have you ever felt lost because it was your first time there? Whether it was an airport, a mall, or a grocery store, hospital. Do you face a problem traveling around a city with ease (maybe if you've just moved to that city or maybe you just are stuck in traffic?). 
It is a general problem that one feels unfamiliar with the procedures to be followed there. Furthermore, it is hard to find particular things such as Information Desk or Restrooms. Worse case, the person may have disabilities like blindness or muteness. 
GPS navigation may help you in getting from one place to another, but it can't be specific to guide you through every single building in the entire city and sometimes can't really help people who have disabilities. 
Who can possibly be our hero?

## What is Wall-E

Wall-E is an IoT robot that helps people who have disabilities or who are new to places in guiding them outdoors and indoors using project tango mapping. Wall-E is designed to bring out the best of the current technologies: once a person initializes the path, the robot can automatically find its path when someone requests. That is, when Wall-E asks, "Where would you like to go?" a person could say "bathroom", or "the ford desk" or even "remote controller and rather than going there yourself it can help you in guiding you through all the straights and turns with you either following it by walking or sitting in it.

## Architecture behind Wall-E ? 

Our team integrated a handful of top-notch technologies, including Intel Edison (2015, quad-core, RAM 800 MHz, max 8GB memory), Google Project Tango (2014, computer vision tablet that understands positions relative to the world around it), web-services via Node.js, and motor sensors. First, the facility managers (i.e. airport person, home owner, etc. ) must know where most things are at. Then he needs to start collecting location data by walking from the "base point" to each destination points. The pre-loaded locations are stored via "data acquisition mode" on the Tango tablet. Wall-E is smart, so he will remember every path you went to grab "that thing" you needed. Note: the wheels and Edison Board were far smaller than Tango tablet, so we added a sturdy tablet holder with compostable cardboard box pieces. 3D Printing (Makerbot Replicator) and industrial design methods were involved.

For users, who is likely new to the place or someone with discomfort, they will easily find Wall-E at the most visible, public area. Wall-E holds the android tablet, Tango, and it will periodically ask "Where would you like to go?" The user will then tell the desired destination, and the bot will guide him to most anywhere. The speech-to-text is enabled via built-in Speech Recognition API, which will then get the location amongst the list of all the previously addressed places. When the mini-adventure is activated, Tango shoots out the signal to the web server, which then alerts to guide the guest to the place! And Intel Edison starts the bot into action. With our precise distance and angle controls, Wall-E will work out its wheels and power to get him there! For the wheels, the two 1kW DC brushless motors are used, which are similar to the ones used in electric chairs. For the power bank, Wall-E runs on a 2 kW battery as soon as the bot is placed in its charging spot. While in motion, Wall-E will not blink even a second to ensure there is no unexpected object interrupting us. If there is, Wall-E will pause you for a moment. Voila, we are never lost!

## Any challenges?
1. Connecting to the internet was unavailable for Raspberry Pi, so we switched to Intel Edison board -- even better performance!
2. Calibrating two different motor wheel performances -- one was slower, so we had to balance the Left & Right motor speed.
3. Connecting to the Bluetooth via Intel Edison board took much longer than we expected (5+ hrs), so we changed the environment to web services.
4. Robot usability -- we envisioned Wall-E to be like "R2D2" from Star Wars or "Wall-E" from Wall-E movie; however, the limited time and knowledge did not allow us to fully expand our ideals. We still kept the touch screen and mobility features that we planned to do!
5. Mobile app platform -- originally planned to do an iOS app that gets voice commands and Bluetooth signal to the embedded processor, but it was much simpler to directly create an Android app onto Tango. 

## Proud moments?
1. Finishing the hack! 
2. Connecting everything into IoT: Intel Edison board (motors, processors) - Web server - Android app - Tango initial mapping 3-axial accelerometer or real-time obstacle detecting integration.
3. Solving how to control motor sensors via distance/seconds unit and trigonometry calculations
4. Allowing Wall-E to be utilized for so many uses: city tour guide replacement, shopping guests in big stores, passengers in train stations or airports, new students at a school, assistance dog alternative for the blinds, a big mansion guidance without a butler, and etc. 


## Lessons we've learned.
1. Never stop finding our way -- with hearts of ambition and passion, we can find a way
2. Hardware integration takes careful attentions and details
3. Flexibility in many computer languages is always helpful
4. Minimum Viable Product methodology is wise and efficient
5. Caution in 3D Printing -- to always think in three dimensions
6. Setting Bluetooth connection takes extra steps
7. How to implement navigation throughout the city (indoors as well as outdoors) using project tango mapping.

## What's next?
1. Add a comfortable seat so that one can conveniently sit and watch, as Wall-E finds the path
2. Bluetooth between Tango and Intel Edison board -- faster connectivity
3. Add on the design aspects for the Android app and the robot
4. Beeping alerts when in guidance (ex. beep for easier follow rather than listening to the motor sounds, beep when obstacles, ask questions for friendliness of the robot)
5. Better motor controls (i.e., non-90-degree rotations of all times, various speed controls, flexibility in rough floors)
6. Larger data handling (with mapping an entire city with every single building) for better flow of people as well as lesser traffic on road.
7. Replacement of the amount of the current on road cars and regulation of flow of not only traffic but even people.

## Links:
1 min, https://youtu.be/2R5CCwQQUP0?list=PLw3XL9sPIofnI1y1Xrt28RenZR0pmfIGO
30 seconds, https://youtu.be/prjxgRk3BnE?list=PLw3XL9sPIofnI1y1Xrt28RenZR0pmfIGO
