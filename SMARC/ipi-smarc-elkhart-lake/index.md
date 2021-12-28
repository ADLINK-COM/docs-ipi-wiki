# Introducing the I-Pi SMARC

When microcontroller development platforms like the Arduino and Raspberry Pi (RPi) first appeared on the scene circa 2005 and 2012, respectively, they were generally regarded as being of interest only to students, hobbyists, and makers.

Over time, however, the open source nature of the hardware and software associated with these platforms – coupled with the huge hardware and software ecosystems that evolved around them – resulted in professional engineers using them as low-cost evaluation platforms for sensors, actuators, and peripherals, and as prototyping platforms for next-generation embedded systems and Internet of Things (IoT) devices.

By the start of 2020, it was estimated that at least **50 million** RPi platforms had been sold in around ten different models/versions. By comparison, there are around 20 different Arduino platforms, some with multiple versions. Unfortunately, there is no accurate record as to how many Arduinos have been sold. If only “official” systems are counted, then the number of Arduinos is probably less than that for the RPi; if unofficial clones are also accounted for, however, then the number of Arduinos almost certainly exceeds that for RPi platforms.

## Prototyping to Production Problems

Engineers are driven to create. Many engineers work with hardware and software in their own time, experimenting at home with peripherals and sensors, and developing prototype versions of potential products. Due to the low cost of entry, they often use Arduino or RPi development boards as their prototyping platforms of choice.

In addition to the open source nature of these platforms, Arduino shields and RPi HATS are available with almost every sensor, actuator, and peripheral one can dream of.

Unfortunately, problems arise when the efforts the engineers have undertaken at home arrive at work, at which time their prototypes need to be translated into industrial solutions. As one simple example, Arduino and RPi platforms are commercial products designed to support commercial temperature ranges and environments – they aren’t intended for use in hostile environments that feature shocks, vibration, noisy power supplies, high humidity, and extreme temperatures.

Another issue is that the creators of products intended for the consumer market – like the Arduino and RPi development boards – are happy to change components and make substitutions as and when circumstances dictate (“these are both 10pF ceramic capacitors, so there won’t be a problem if we use them interchangeably”). This philosophy is unacceptable in the case of products intended for medical, industrial, or military use.

*The bottom line is that it simply is not possible to “drop” an Arduino or RPi prototype into a box and call it an industrial solution.*

By comparison, ADLINK’s I-Pi SMARC follows industry standard **ECN** (engineering change notice) and **PCN** (process change notice) practices, which means that end users have access to an audit trail that defines what changes, if any, have *been* made and why those changes *were* made. (ECNs are items that affect the fit, form, or function of the product; PCNs are changes to how the product is made.)

There are, of course, many existing industrial platforms available, but they each have different register maps and hardware interfaces when it comes to talking to things like general-purpose input/output (GPIO) pins, pulse-width modulator (PWM) functions, analog to digital converters (ADCs), digital to analog converters (DACs), and communication functions like I2C, SPI, UART, etc. This makes it difficult to take the software and drivers developed for an Arduino or RPi and migrate them to an industrial platform.

The [MRAA](https://github.com/eclipse/mraa) (pronounced “em rah”) library on the I-Pu SMARC simplifies the logic for connecting to different sensor pins. In addition to allowing users to program in C++, Python, JavaScript, Java, MRAA is portable, thereby allowing the same code to be run on multiple platforms.