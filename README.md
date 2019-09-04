## Inspiration
We wanted to make a project that was a culmination of various hardware and software skills that we acquired in school and we were inspired by the fire alarm episode from The Office and seeing everyone go into panic because of the fire made us realize that having a fire detector that would've called 911 for them automatically would have gotten firefighters on the way to the fire while everyone was panicking and trying to get out the building. So we decided that making a smart fire detector was a perfect combination of our skills and has the potential to be accessible and used everywhere. The fire detector costs $56.21 in parts and has the potential to be cheaper with more time and development.

## What it does
The fire detector reads a thermal and a smoke sensor from the Arduino to look at levels of smoke and ambient temperature. The idea is that smoke detectors just detect smoke which doesn't always mean there's a fire. So having a thermal sensor as well would help with confirming there is a fire and reduce false alarms. When the sensors indicate that there's a fire it will ring a buzzer to notify the people around, it will send a text message to the owner, and call 911 reporting a fire at the address of the fire detector.

## How we built it
Starting from the sensor modules, we used a temperature sensor and a CO2 sensor. We then connected those to an Arduino that would read the sensor data. From there, we connected the Arduino to a Raspberry Pi, and configured the Raspberry Pi to read serial output from the Arduino. The Raspberry Pi then reads the serial output and triggers a script to run once a specific parameter has been met, and that script uses an API to send a text and phone call to the recipient(s).

## Challenges we ran into
Some of the challenges we ran into were calibrating the sensors to be a perfect balance of proactive and reactive. We wanted to make sure it detects actual fires and wouldn't produce false alarms. We also ran into issues with converting the signals we were getting in voltage and making them readable in Fahrenheit. Another issue was integrating all the individual components and getting them to work with one another.

## Accomplishments that we're proud of
We're really proud of getting the hardware reading the different sensors, especially considering that none of us knew how to do that before the project. We're also proud that we were able to implement both hardware and software aspects of the projects into something that can truly make a difference and be accessible by everyone.

## What we learned
NOT TO PUT API KEYS ON GITHUB!!! We learned about how to have the Arduino and Raspberry Pi communicate with each other, and how to integrate python code to access hardware things as well. We also learned a lot about fire statistics and how smoke detectors work. 

## What's next for Houston-Hackathon-Smart-Fire-Detector
We'd like to fine-tune our product and work with local government to see if this is something we can implement and make accessible for everyone!
