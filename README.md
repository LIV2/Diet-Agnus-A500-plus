# Diet Agnus A500+ 8372A Adapter

The 8375 Agnus needed for Amiga 500+ is getting expensive and scarce so this adapter is designed to allow you to fit the much more common 8372A and other 1MB Agnuses from the A500
It also has the ability to take 1MB of DRAM on board instead of the harder to source DIP20 DRAMs needed for an Amiga

PCBs are available at [Bobs Bits](https://www.tindie.com/products/bobsbits/diet-agnus-adapter-by-liv2/)

### Frequently Asked Questions:
Q. Will this give me 2MB chip ram?<br />
A. No, the 8372 Agnus supports a maximum of 1MB chip ram

Q. Does my Amiga need any ram chips on-board?<br />
A. If you fit the RAM chips specified to the Diet Agnus adapter then your mainboard needs no working chip ram (So if you're building an [A500++](https://www.tindie.com/products/bobsbits/a500-amiga-500-replica-pcb/) you can leave those out)

![PCB](PCB.png?raw=True)

### Assembly Steps
1. Solder the DRAMs (or if using the Amiga's ram, cut and set the jumpers to "Enabled" and go to step 3)

2. Solder the Capacitors (Only fit VBB capacitor if your Agnus says VBB on the top)

3. Solder the PLCC Socket making sure that the socket aligns exactly with the outline on the top of the PCB!

4. After soldering the socket, you may want to trim the joints down to the PCB to make soldering the pin headers easier. <br/>**Be careful when trimming the leads that you don't scratch the PCB solder mask!**
 
5. Prepare the pin headers by removing a pin from this corner of each as indicated here:<br/>
![remove](Images/header.png?raw=True)
6. Insert one of the pin headers just far enough for it to hold, making sure that it is level.<br/>
The side with the removed pin goes where indicated by the yellow arrow<br/>
I recommend doing them one by one in the order indicated:<br/>
If you will be soldering to the Amiga rather than using sockets, I would recommend soldering the long side of the pins to the adapter
![locations](Images/locations.png?raw=True)
![insert](Images/insert.png?raw=True)

7. Solder in each pin, don't use too much solder!

8. Repeat for each pin header<br/>
![solder](Images/solder.png?raw=True)


### Installation
You will need to remove the Agnus socket from your Amiga PCB and solder female pin headers in it's place (making sure to remove the corner pins of the pin header) or solder direct in place of the Agnus socket.

The board must be oriented so that the RAM sits to the right of Agnus, with Agnus' pin 1 pointing to the right

## NTSC
Close the NTSC jumper to set your Agnus to NTSC mode (Only if the Agnus isn't marked with VBB!)

## Jumpers
The "Amiga RAM" jumpers control whether the various RAM control signals are routed to the Amiga's original ram or to the ram chips on the board.

If you have fitted the 2 RAM chips to this adapter you must leave the jumpers at the default setting.

If you instead want to make use of the Amiga's RAM chips you can cut and set all 4 of the jumpers to "Enabled" and leave off the 2x ram chips.



### Bill of materials
|Component|Location|QTY|Link|
|---------|--------|---|------|
|Diet Agnus PCB| |1|[Bobs Bits](https://www.tindie.com/products/bobsbits/diet-agnus-adapter-by-liv2/)|
|Ceramic Capacitor, 0.1uF, 0805|C1-7|7|[Mouser](https://www.mouser.com/ProductDetail/710-885012207098)|
|PLCC-84 Socket, Through-hole|U1|1|[Mouser](https://www.mouser.com/ProductDetail/437-5408808424008) |
|5V, 256Kx16 EDO/FPM DRAM, SOJ-40 (e.g HYB514171BJ)|U2-3|2|eBay, Aliexpress etc|
|22-Pin, 2 Row Female header||4|[Mouser](https://www.mouser.se/ProductDetail/517-929975-01-11-RK)
|22-Pin, 2 Row Male header||4|[Mouser](https://www.mouser.se/ProductDetail/649-77313-118-22LF)
