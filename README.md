# Design of RF Mixer Circuit Using 28 nm CMOS Technology
# Abstract
Frequency translation which converts the original signal to a much lower baseband frequency signal is a vital role in the RF receiver design. In this work, a down-conversion Gilbert cell mixer is designed using 28 nm RF CMOS process. The mixer covers the frequency band of 3.1-9.5 GHz. The RF mixer provides the high conversion gain with low noise figure at 100MHz IF.
# Introduction
Federal Communication Commission introduced Ultra Wide-Band technology in the frequency range of 3.1-10.6 GHz for unlicensed use [1]. The down conversion mixer is an important component in RF receiver front-end which is shown in Figure 1. The mixer is used as a frequency translation device which down converts the Radio Frequency (RF) signal passing through Low Noise Amplifier (LNA) into Intermediate Frequency (IF) signal. The CMOS technology is used to implement it. The RF parameters such as conversion gain, noise figure and power consumption are important for mixer design. 
Mixers are used for frequency translation i.e. they are used to convert the RF signal (incoming signal after it is amplified by the LNA) to an intermediate frequency (IF) by multiplying it with a local oscillator (LO) signal. The block level representation is shown in Figure 2. The intermediate frequency can be the sum of frequencies of the two input signals or can be the difference between the two signal frequencies.
# Tool Used
Compiler: Synopsys Custom Compiler

PDK: Synopsys 28 nm CMOS Technology
# Design of RF Mixer Circuit
The conventional Gilbert cell mixer shown in Figure 3 consists of three stages such as Transconductance stage, Mixing stage and Load stage. The RF input signal is given to transconductance stage acting in saturation region where the RF voltage is converted into RF current. 
The mixing stage is acting in triode region that performs switching by LO signal.    The conversion gain ( ) expressed in Equation (2) is proportional to the transconductance of the transistors.
 
 * RF Mixer Circuit
 
 ![Model](I:\sairam\Sairam\IITHakathon\RFMixer.png)
 * Schematic Diagram
 * Primewave Setup
 * Testbench Waveform
# Reference
[1]	First report and order, revision of Part 15 of the commission’s rules regarding ultra wideband transmission systems,  FCC, Washington, DC DC ET Docket, 98-153,2002.

[2]	Behzad R. (2012). RF Microelectronics (2nd ed.). Prentice Hall: Englewood Cliffs. 

[3]	Han, G., & Sanchez-Sinencio, E. (1998). CMOS transconductance multipliers: A tutorial. IEEE Transactions on Circuits and Systems II: Analog and Digital Signal Processing, 45(12), 1550–1563. 

[4]	Kan, K., Ma, D., & Luong, H. (2000). Design theory and performance of 1-GHz CMOS downconversion and upconversion mixers. Analog Integrated Circuits and Signal Processing, 24(2), 101–111
