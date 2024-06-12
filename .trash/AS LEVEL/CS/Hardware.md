# Memory
![[Memory.excalidraw]]
## Primary Memory
| <font color="#00b050">RAM                        </font>| <font color="#938953">ROM</font>                     |
| -------------------------- | ----------------------- |
| Temporary                  | Permanent               |
| Stores data of apps in use | Stores Boot Information |
| Volatile Memory            | Non Volatile            |

### Ram Ram

| **DRAM**                            | **SRAM**                            |
| ----------------------------------- | ----------------------------------- |
| Needs to be refreshed               | No need to be refreshed             |
| Less expensive                      | More expensive                      |
| Uses 1 capacitor & 1 transistors    | Uses Flip flops (Memory Cell)       |
| Capacitors hold 1/0                 |                                     |
| Transistors act as switch           |                                     |
| Takes about 60 nanoseconds to fetch | Takes about 25 nanoseconds to fetch |
| Recharge every 15 microseconds      | No frequent recharge                |
| Uses more power than SRAM           | Uses less power than DRAM           |

### ROM ROM
- ROM - Read Only Memory
- PROM - Programable Read Only Memory
	- Found in mobiles/RFID
	- Matrix of fuses
	- Can be changed once
- EPROM - Erasable Programable Read Only Memory
	- Found in game consoles under development
	- Transistors and Capacitors
	- requires UV light to modify
	- can be changed once
- EEPROM - Electrically Erasable Programable Read only Memory
## Secondary Memory 
### HDD vs SSD
| HDD                      | SSD                   |
| ------------------------ | --------------------- |
| Uses magnetic properties | Uses flash technology |
| Contains moving parts    | No moving parts       |
| Very noisy               | Quiet                 |
| Less durable             | Highly durable        |
| Heavy and bulky          | Light weight          |
| Uses tracks and sectors  |                       |
| Very cheap               | More expensive        |

![[hdd-ssd.excalidraw|800]]
#### HDD working
- The hard disk has one or more platters made of aluminium or glass
- Each surface Of the platter/disk is ferrous-oxide which is capable Of being magnetised
- The platters/disks are mounted on a central spindle
- The disks are rotated at high-speed
- Each surface of the disk has a read/write head mounted on an arm positioned just above the surface
- Electronic circuits control the movement of the arm and hence the heads
- The surface of the platter/disk is divided into concentric tracks and sectors
- One track in one sector is the basic unit of storage called a block
- The data is encoded as a magnetic pattern for each block
- When writing to disk, a variation in the current in the head produces a variation in magnetic field on the disk
- When reading from disk, a variation in magnetic field produces a variation in current through the head
### CD, DVD, Blu-Ray
#todo ^
### Reading a drive:
- Drive motor is used to spin the disc
- Tracking mechanism moves the laser assembly
- A lens focuses the laser onto the disc
- Laser beam is shone onto disc to read / write
- Surface of disc has a reflective metal layer / phase change metal alloy
- Track(s) on the disc have sequence of pits and lands / amorphous and crystalline state
- Reflected light in then encoded as a bit pattern
- #### Use cases
- Additional File storage
- Backup  of files
- Archival of files
- Transfer to another device
### Pendrives
#todo ^
# Printers
| **Laser Printer**                      | **Inkjet Printer**                           |
| -------------------------------------- | -------------------------------------------- |
| Higher initial cost                    | Small initial cost                           |
| Good long term cost                    | Costly to refill                             |
| Uses powder/toner                      | Uses liquid Ink                              |
| Low Quality compared to inkjet         | High Quality                                 |
| Large Buffer Memory, stores whole page | Small Buffer Memory store one line at a time |
| Fast Printing                          | Slow Printing                                |
| Ozone Irritation                       |                                              |
|                                        |                                              |
![[Pasted image 20231219192124.png]]
## Laser Printer 
#### LP print cycle
1. Laser beam and a rotating mirror are used to draw an image of the page on the photosensitive drum
2. The image is converted on the drum into an electrostatic charge
3. Electrostatic charge attracts toner
4. Charged paper is rolled against drum
5. The oppositely-charged paper picks up the toner particles from the drum. After picking up the toner, the paper is discharged to stop it clinging to the drum
6. The paper passes through a fuser, which heats up the paper. The toner melts and forms a permanent image on the paper.
7. The electrical charge is removed from the drum and the excess toner is collected
## Inkjet Printer
#todo inkjets
#### Print Head:
- The print head contains a large number of very small nozzles
- Ink is fed to each nozzle from a reservoir
- The print head fires droplets of ink onto the paper
- The print head moves horizontally across the paper
- Replacement ink fills the nozzle
#### Stepper Motor
- The (print head) stepper motor is connected to the print head by a belt
- The (print head) stepper motor moves the print head across the paper
- The (parking) stepper motor parks the print head assembly when not in use
- The (paper feed)stepper motor turns the rollers that provide the paper feed // The (paper feed)stepper motor moves the paper in small increments
### Piezoelectric
### Thermal bubble
# 3D printer
- Uses CAD

# Speakers
### Parts of a speaker:
1. Diaphragm/Cone
2. (Voice) Coil of wire
3. Spider/Suspension
4. Permanent Magnet
5. Basket
6. Dust Cap
7. Outer Frame
### Working of a speaker:
1. Takes an electrical signal and translates it into physical vibrations to create sound waves
2. An electric current in the coil creates an electro-magnetic field
3. Changes in the audio signal causes the direction of the electric current to change
4. The direction of the current determines the polarity of the electro-magnet // changing the direction of the current changes the direction of the polarity of the electro-magnet
5. The electro-magnet is repelled by or attracted to the permanent magnet causing the coil to vibrate
6. The movement of the coil causes the cone / diaphragm to vibrate
7. That vibration is transmitted to the air in front of the cone / diaphragm as sound waves 
8. The amount of movement will determine the frequency and amplitude of the sound wave produced              
# Microphone 
#todo microphone

# Screens

| LCD           | LED | OLED                    |
| ------------- | --- | ----------------------- |
| Cheap         | Mid | Pricey                  |
| Backlight LED | LED | Foldable to some Degree |
## LCD 

## LED
## OLED

# Rest of the Hardware components
## Keyboards:
- Uses switches and circuits to translate keystrokes into signals the computer can understand
- The key matrix is a grid of circuits / three layers of plastic underneath the keys
- Each circuit is broken beneath the key / middle layer contains holes
- When key pressed, a circuit is made / completed and a signal is sent
- Processor compares location of signal from key matrix to a character map stored on
- ROM
- A character code for each key press is saved in a keyboard buffer
## Optical Mouse:
- Laser / light shines onto a surface
- Through a (polished) ring at the base
- The light is reflected from the surface through the ring
- Sensor detects reflected light
- Capturing details / photograph of surface (under the ring)
- At about 1500 times per second
- As the mouse moves the sensor detects changes in the surface detail / photograph
- Which are translated into movement (change of x and y co-ordinates)
- The processor/software updates the position of the cursor on the screen
## Scanner:
- Main component Of a scanner is a CCD array
- CCD is a collection of light sensitive diodes
- Laser beam / light is shone onto the source document/barcode
- The scanned image reaches the CCD through mirrors and lenses
- Sensors detect levels of reflected light
- Brighter light results in greater electrical charge
- Light intensity is converted (by software) to a digital value
# Monitoring system
1. Sensor makes a measurement
2. Data is converted to electrical signal with ADC
3. Microprocessor calculates the data
4. If data is within parameters loop continues else
5. If not then signal is sent to {destination}
