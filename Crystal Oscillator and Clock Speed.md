## Crystal Oscillator

Integrated on the mother board, used to control the rate of the instructions to be executed

### Clock Speed

Crystal oscillator vibrates when an AC (Alternating Current) is applied to it, the vibration is then converts to a varying output voltage that has 100 million cycles in a second and it is equal to a frequency of 100 MHZ(megahertz). The time for one cycle can then be calculated as 10 ns(nanoseconds) and this is called the ===base clock frequency===.

Special circuits inside the CPU called the <u>frequency dividers</u> and <u>frequency multipliers</u> takes the reference of signal and multiply it up to a much higher frequency that controls the rate of instructions are executed.

Ex. Multiply the base clock signal by 35 can give a frequency of 3500 MHZ and is equivalent to  3.5 GHZ(gigahertz) which is a typical CPU clock frequency.

![[Pasted image 20221028190255.png]]
### Component Specific Clock Speed

Other computer components can run at different rates to the CPU cores by dividing or multiplying the base clock frequency according to their own needs.

Ex. Multipliers inside the memory controller can generate a different frequency to control the rate at which the data moves on the memory bus. A memory bus designed to support DDR4 DRAM typically operates at the frequency of about 1.2 GHZ


### Overclocking

A modern CPU can dynamically change its clock speed depending on the task it's performing. For demanding tasks it can temporarily raise the clock frequency to get things don quicker, it can also throttle down the frequency if it starts getting too warm.

A good cooling system can allow a CPU to perform tasks at high speed for longer period of time.

If a CPU's frequency multipliers have been unlocked then its possible to increase the clock rate to exceed that certified by the manufacturer. This is called overclocking.

When it comes to comparing CPU performance, it needs to multiply the clock speed by the number of cores and by the instruction rate of each core.