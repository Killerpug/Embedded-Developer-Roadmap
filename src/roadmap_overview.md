# Roadmap Overview


```plantuml,format=svg
@startuml
skinparam linetype polyline
'skinparam linetype ortho

/' ******************************* Start Fundamentals ****************************** '/
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

class "Control Engineering" as control_eng {
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



/' ******************************* Finish Fundamentals ******************************'/


/' *********************************** Start Tracks ********************************'/

struct "Tracks" as Tracks {

}



class "Machine Learning " as machine_learning {
  + Fundamentals
}

class "Cybersecurity " as cybersecurity {
  + Fundamentals
}

class "Firmware " as firmware {
  + Fundamentals
}

class "Internet Of Things " as iot {
  + Fundamentals
}

class "Systems Control" as sys_control {
  + Fundamentals
}

class "Embedded Linux" as embedded_linux {
  + Device Drivers
}

class "Audio" as audio {
  + Fundamentals
}

class "Radio Frequency" as radio_frequency {
  + Fundamentals
}

class "Software" as embedded_software {
  + HW emulators
  + RTOS
}

class "Tester" as tester {
  + Fundamentals
}

class "Validation" as validation {
  + Fundamentals
}



/' *********************************** Finish Tracks ********************************'/


/' *********************************** Start Industry_applications ********************************'/

struct "Industry applications" as Industry_applications{

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

class "Drive by Wire" as drive_by_wire{

}

class "Flight Recorder" as flight_recorder{

}



struct Biomedical {
   
}

class "Imaging" as imaging {
   + X-ray
   + 3D models
   + QNX()
}

class "smart prosthetics" as smart_prost {
  + brain-controlled
  + exoskeletons
  + nerv-controlled
}

class "medical instrumentation" as medical_instrumentation {
  + measurement: blood pressure, hearth rate, /n
   oxidometer, spirometers.
}


struct "Consumer Electronics" as Consumer_Electronics {
   + Home appliances
}

class "wireless communications" as wireless_comms{
   + RF: 4G, 5G, LTE
   + wifi
}

/' *********************************** Finish Tracks ******************************** '/

Fundamentals -u-> circuits
Fundamentals -l-> math
Fundamentals -r-> digital_sys
Fundamentals -r-> data_algo
digital_sys -r-> os
digital_sys --> comp_arch
math -l-> control_eng

Fundamentals --d-> Tracks

Tracks -l-> audio
Tracks -l-> cybersecurity
Tracks -l-> embedded_linux
Tracks -l-> embedded_software
Tracks -l-> firmware
Tracks -r-> iot
Tracks -r-> machine_learning
Tracks -r-> radio_frequency
Tracks -r-> sys_control
Tracks -r-> tester
Tracks -r-> validation

Tracks --d-> Industry_applications

Industry_applications --> Automotive
Industry_applications --> Aerospace
Industry_applications --> Biomedical
Industry_applications --> Consumer_Electronics
Aerospace --> drive_by_wire
Aerospace --> flight_recorder
Aerospace --> wireless_comms
Automotive --> drive_by_wire
Automotive --> gateways
Automotive --> infotaiment
Automotive --> driver_assistance
Automotive --> wireless_comms
Biomedical --> imaging
Biomedical --> smart_prost
Biomedical --> medical_instrumentation




@enduml
```

What is the recommended usage of this roadmap?
1. Complete the Fundamentals, this is knowledge that will be the pillar for anything you may end up working on as an Embedded Developer and even most of it applies to other engineering branches.
2. Select one Track and one Industry that catches your attention and start getting familiarized with the topics inside of both, for example: My goal is to learn about Embedded Software track in the Automotive Industry, If you were to select gateways then you could become proeficient in handling and passing data between two components.