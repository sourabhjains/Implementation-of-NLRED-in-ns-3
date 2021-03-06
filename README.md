# Implementation of Nonlinear RED (NLRED) algorithm in ns-3
## Course Code: CS822  <br/>                  
## Assignment: #GP1    <br/>

### Overview           <br/>

Nonlinear RED (NLRED) [1] is a variant of Random Early Detection (RED) [2] in which the linear packet dropping function of 
RED is replaced by a nonlinear quadratic function. This repository provides an implementation of NLRED in ns-3.25 [3]. <br/>

### Simulating NLRED	<br/>

To simulate NLRED algorithm, the attribute NLRED must be set to true,
as shown below:

  `Config::SetDefault ("ns3::RedQueueDisc::NLRED", BooleanValue (true));`

### NLRED example	<br/>

An example program for NLRED has been provided in

`src/traffic-control/examples/red-vs-nlred.cc`

and should be executed as

`./waf --run "red-vs-nlred --queueDiscType=NLRED"`

### References         <br/>

[1] Kaiyu Zhou, Kwan L. Yeung, Victor O.K. Li (2006). Nonlinear RED: A simple yet efficient active queue management scheme. <br/>

[2] Floyd, S., & Jacobson, V. (1993). Random early detection gateways for congestion avoidance. IEEE/ACM Transactions on networking.<br/>

[3] https://www.nsnam.org/ns-3-25/

