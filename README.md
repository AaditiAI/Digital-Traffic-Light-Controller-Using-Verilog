## Digital Traffic Light Controller Using Verilog
## Introduction
This project implements a Digital Traffic Light Controller using Verilog HDL (Hardware Description Language). The controller is designed to manage the traffic signals of a highway (hwy) and a country road (cntry) in a simple intersection. The traffic lights follow a timed state machine with green, yellow, and red signals, ensuring smooth and regulated traffic flow.

### Features
Timed Signal Transitions: The traffic light transitions from green to yellow and red, based on pre-defined delays.
Highway and Country Road Signals: Controls two sets of traffic lights for the highway and country road.
State Machine Based Design: Implements a finite state machine (FSM) to manage the state transitions.
Responsive to External Input: The system can adjust based on external input (X), indicating whether traffic is present on the country road.

### State Machine Design
The traffic light controller operates in five states:
S0: Highway green, country road red.
S1: Highway yellow, country road red.
S2: Highway red, country road red.
S3: Highway red, country road green.
S4: Highway red, country road yellow.
The transition between states is triggered based on delays (Y2RDELAY for yellow-to-red, R2GDELAY for red-to-green) and the presence of vehicles on the country road (input X).
