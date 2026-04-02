# Femto-Lite v1.0.0 (Updated 02APR26 APM)

**Written by:** Adam Micolich

## Contents of the *PCBs & Schematics* folder

There is a single PCB in the Femto-Lite. The various files and folders are as follows:

`Femto-Lite Schematic.pdf`: The schematic diagram for the circuit used in this box.

`Femto-Lite PCB Design.pdf`: PCB design shown to actual size.

`Femto-Lite Parts List.pdf`: Parts list for all the components needed for assembly.

`Femto-Lite Assembled 1.jpeg`: Photograph of an assembled Femto-Lite with top panel in place.

`Femto-Lite Assembled 2.jpeg`: Photograph of an assembled Femto-Lite with top panel removed.

`Femto-Lite Specs.pdf`: Plots of output voltage vs input current for the two gain settings 1000V/A and 10000V/A.

*Gerber Files*: A folder containing all the Gerber files needed to have these PCBs produced. It is a fairly standard two-layer PCB.

We get these PCBs made for us by PCBWay in China.

## Brief discussion of the circuit design aspects for the Femto-Lite

The Femto DLPCA-200 current pre-amplifier has long been used in electrical measurement setups at UNSW, often for measuring current signals that simply don't require the performance (and the price it entails) provided by the DLPCA-200. This instrument was designed to provide a simple, low-cost two-channel equivalent of a Femto DLPCA-200 for the measurement of d.c. and quasi-d.c. currents in the mA to high uA range.

The circuit centres on a traditional transimpedance amplifier circuit using the Texas Instruments TLV2721 Op-amp. The circuit is designed with two gain settings 1000 V/A and 10000 V/A that can be switched between using jumpers. Notionally, other gains could be obtained simply by replacing the feedback resistors on the op-amp, which are simply precision 0805 SMT resistors.

The circuit is powered using a USB-C power supply, which is fed into an isolated dc-dc converter to provide +/-5V rails for the op-amp, such that the amplifier can work bipolar rather than unipolar. As such, the voltage outputs saturate at around 5V -- there is no overload circuitry in order to keep costs down, so a user needs to be cognizant of ensuring the input signal does not become to high. Breaking the circuit is unlikely unless the current overload is severe, the measurement will just be 'clipped'.

The remaining jumpers are provided for grounding versatility (e.g., noise optimisation). There are two banks of screw-terminals on the board for the BNC connections -- note that each of these appears twice in the schematic to enable the connections to be properly mapped, the BNC connections come in at the screw-points, the circuit connections are the solder pins, respectively.

The circuit behaves with good linearity to almost zero input current. Note that the output voltage is the opposite sign of the input current, an inherent aspect of the transimpedance amplifier, where V_out = -I_in/R_F where R_F is the feedback resistance.
