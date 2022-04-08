## Hints Dont forget to add some pictures for <br >01- beaglbone<br > 02- Intell galilio <br >03- Ti <br >
# What is new in ARM processor
ARM contains core prepherials exists in the processor <br >
01- NVIC      Nested vector interrupt controller<br >
02- SYSTIC    Timer inside the processor 24 bit <br >
03- MPU       Memory protection unit<br > 
04- ICD       in circuit debugger<br >
### Data buses <br >
01- Address bus<br > Bus neededd to address specific address
02- Data bus<br > Bus needed to transmit or receive data
03- Controll<br > bus Bus needed to send controll commands 
Bus set is a set of data, controll and address buses 
### Harvard Vs Vonnumen architecture
***Harvard is complex !***
Harvard has different asembly instructions for accessing specific bus set
if code in c then the diffult access is RAM bus set  
### Pipeliming concept 
in Harverd architecture there is different bus set for proividing excution of more than one instruction cycle at same time 

ARM Mix between harvard and von-numen
## Questions 
What is the difference between instruction cycle , clock cycle and machie cycle <br >
Clock cycle it generated from clock in hz<br >
Machine cycle the actual clock after prescaller<br >
instruction cycle number for cycle for fetching decoding and excuiting the instruction<br >
[Note]  
16/32 bit instruction is called thumb2 
insurction can be fetched in morethan one cycle for ASK ?

## ToDo
Cemsis<br >
Eclipse debugging <br >
Outlines <br >
## Lec2
***processor*** <br >
Each proecessor Control unit contains a fetching circuit for fetching the instruction and understand it using instruction format and instruction set to decode the instruction then the decoded instruction is enter to ALU to be excuited for op1,op2 and opcode which will be in the selector and then the result will bw in the accumulator <br >
***Memory*** <br >
Development time : Time of development 
Building time    : Time of building the code to get hex 
profiling        : getting memory size needed for uploading the code
Flashing         : Time of burning or flashing the code using flasher or programmer 
The code is represented in the memory using electrical signal on or off zero or one 
Memory can be implemented using:<br >
01- Capacitor  : Charged then one represented in the memory <br >
02- Transistor : Saturation mode "short circuit" which represent 1 
Open circuit mode "represent zero"

|Comparassion       |Transistor           | Capacitor      |
|----------|------------------------------|----------------|
|  Performande         |High                              |Low            |
|  Cost        |High                              |Low                |
|  Size        |Low                              |High                |
|  Power Consum.        |Low                              |High                |
|  Name.        |SRAM                              |DRAM                |

Cpacitor consume a high power because  a refreshment circuit is needed to save charge 
Note: Both DRAM And SRAM are volatile and will not save code text in the flash memory so a 
<br >***floating gate mosfet is needed***<br >
floating gate mosfet is non volatile 
01-Control gate: which receive the signal to be applied on the mosfet and need to be high power to penetrate isolator<br >
02-Isolator     : Exist between control gate and floating gate<br > 
03-Floating gate: a gate which hold the signal between source and drain<br> 
04-Source: like collector of transisor<br >
05-Drain : like transistor collector <br >
if ther a charge stored in the floating gate then Retention time will be 50 years and then it will lose it's charge 
Float gate mosfet may be:<br >
 01-charged then applied signal to gate is zerro
 <br >02-Not charged then applied signal to gate is 1
<br >Note : when the memory is cleared then it will contains ones 
Disadvantages of floating gate mosfet:
01- Nonvolatile    : Which read only for processor and processor can't write over it 
02- Need High powr : to break floating gate mosfet 
### Memories based on float gate mosfet:
***Masked ROM:***
A memory which come already programed and we can't programe it 
<br >***OTP ROM:***
A memory which can be programed only once by the user  
<br >***EPROM:***
Erasable programable ROM can be programed using burner by electricity and can be erased by ultravilot `Widdly used in weapons manufacturing `
<br >***EEPROM:***
Electricall ersable programble can be programed and erased using electricity
<br >***Flash:***
Electricall ersable programble can be programed and erased using electricity

|Comparassion       |EEPROM           | FLASH      |
|----------|------------------------------|----------------|
|  Accessing[write/erasing]         |Byte access                              |Block access            |
|  Cost        |High[need more transistors to access byte]                             |Low                |
|  Endurance        |100,000 write erase                             |10,000                |


[Note]
To undertand relation between flash and EEPROM <br >
Flash access time for example take   10us <br >
EEPROM access time for example take   1us <br >
Case1: Write one byte ``EEPROM`` Will consume 1us and ``Flash`` will consume 10 us which means EEPROM is faster for byte access 
<br >Case2: Write 100 bytes ``EEPROM`` Will consume 100us and ``Flash`` will consume 10 us which means flash is faster for block access<br >

***conclusion:***<br >
Memory divided into two main types <br >
01-Volatile     : [RAM(SRAM-DRAM)]<br >
02-Non-Volatile : [ROM(MASKED-OTP-EPROM-EEPROM-FLASH)]<br >
