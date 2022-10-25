# Roadmap Overview


```plantuml,format=svg
@startuml
'skinparam linetype polyline
skinparam linetype ortho

struct Fundamentals {

}

class "Data structures and Algorithms" as data_algo {
  + Collections: Linked list, stack, queues, \n
   hash tables, heaps, binary trees
  + Interfaces
  + recursion
  + Sorting
  + Graphs
}

class "Mathematics" as math {
  + Linear Algebra: Factoring, Quadratic formula, Binomial Theorem, \n
    Inequalities.
  + Trigonometry.
  + Geometry: Distance formula, circles, lines,
  + Calculus: limits, functions, derivatives, integrals

}

class "Digital Systems" as digital_sys {
  + Continuous vs discrete systems: Analog vs digital, binary system, \n
   logic functions, boolean algebra digital waveform, data transfer, \n
   combinational and sequential logic, memories, Finite state machines.
  + Build an 8bit computer on FPGA : memory, ALU

}

class "Control Systems" as control_sys {
  + Fundamentals

}


class "Computer Architecture" as comp_arch {
  + Memory Layout()
  + ISA()
}

class "Operating Systems" as os {
  + Programming language
  + pipes()
  + process and threads()
  + concurrency
}


class "System Interfaces" as sys_int{
   + Register()
   + Memory maps()
}

class "Circuits" as circuits {
   + Circuit analysis : current flow, voltage drop, capacitors,\n
    op-amps, diodes, transistors.
   + Sound system() : filters and amplifiers, power sypply.
}

Fundamentals -u-> circuits

Fundamentals -l-> math
Fundamentals -r-> digital_sys
Fundamentals --> data_algo
digital_sys -r-> os
digital_sys --> comp_arch
math -l-> control_sys

struct "Tracks" as Tracks {

}
Fundamentals -d-> Tracks

class "Compiler" as compiler {
  + Bootloader()

}

class "Hardware emulators" as hw_emulator {
  + Fundamentals : NES emulator

}


class "topic " as topic {
  + Fundamentals

}



struct Industries {

}



struct Automotive {
  + MISRA
  + CAN
}




class "Gateways" as gateways{

}
class "Infotaiment" as infotaiment{

}
class "Driver Asistance" as driver_assistance{

}

struct Aerospace {
   
}



class "Coordinated Systems" as coordinated_systems{

}

struct Biomedical {
   
}



class "Medical grade devices" as medical_devices {
   + X-ray imaging
   + Wearable tech
   + QNX() : create a medical grade device with real time constraints.
}



struct "Consumer Electronics" as Consumer_Electronics {
   + Home appliances
}

struct Communications {
   + RF
}

Tracks -d-> Industries
Industries --> Automotive
Industries --> Aerospace
Industries --> Biomedical
Industries --> Consumer_Electronics
Industries --> Communications
Aerospace --> coordinated_systems
Automotive --> gateways
Automotive --> infotaiment
Automotive --> driver_assistance
Biomedical --> medical_devices

@enduml
```

What is the recommended usage of this roadmap?
1. Complete the Fundamentals, this is knowledge that will be the pillar for anything you may end up working on as an Embedded Developer and even most of it applies to other engineering branches.
2. Select one Track and one Industry that catches your attention and start getting familiarized with the topics inside of both, for example: My goal is to learn about Embedded Software track in the Automotive Industry, If you were to select gateways then you could become proeficient in handling and passing data between two components.