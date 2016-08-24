# Overview

The Isolated CANbus BoosterPack provides for a USB to CANbus interface for use in development
of OpenLCB. 

In this document:
 - **Device** is used to refer to the Isolated CANbus BoosterPack.
 - **Assembly** is used to refer to the Device with a Tiva Launchpad attached.
 - **Bus** is used to refer to the OpenLCB CANbus physical layer.

In all specifications:
 - Sentences that use the verb **shall** are absolute requirements. They must be met for
   the design to meet the specification.
 - Sentences that use the verb **should** are desired requirements. They should be implemented
   in the design as long as doing so doesn't violate any absolute requirements.
 - Sentences that use the verb **may** are optional requirements. These can be included
   in the design if possible but not meeting them does not compromise the overall function
   of the device.
 - Sentences *in italics* provide additional information about a requirement such as the
   reason that the requirment exists or how the implementaiton of the requirement should
   be validated.

# Interface Requirements

1. The Device shall implement the CANbus physical layer of the OpenLCB specification.
   *The OpenLCB specification documents can be found 
   [here](http://http://openlcb.com/openlcb-and-lcc-documents/openlcb-specifications/).*

2. The Device shall include a conenctor for an external DC power supply to provide power to 
   the Bus. 

3. The Device shall consume no more than 100mA from the Bus.

4. The Device shall inclue male pin headers for connection to the bootom side of a TI Tiva
   Launchpad EK-TM4C123GXL. The Device should support connection to a TI Tiva Launchpad
   EK-TM4C1294XL.

5. The Device shall provied a minimum of 1kV (RMS) isolation between the Bus and the
   connected Launchpad.

6. The Launchpad and its connected circuitry shall be powered from the attached computer
   via the USB connection.

# Functional Requirements

1. The Device shall be compatible with the OpenMRN software stack. *This stack is hosted
   [here](https://github.com/bakerstu/openmrn).*

2. The Device shall not prevent use of software other than the OpenMRN stack.
