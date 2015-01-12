Implementing Reliable Transport Protocols
=================================

### Description

In a given simulator, implemented 3 reliable data transport protocols ­ Alternating­Bit (rdt3.0), Go­Back­N (GBN), and Selective­Repeat (SR). Understood how AB, GBN, and SR work and compare their performance in the given simulator.

### Program Execution

1) Import the RDT folder into eclipse CDT as a makefile project and compile it													
2) The protocols(ab.c, gbn.c and sr.c) requires two arguments:

● Seed: The simulator uses some random numbers to reproduce random behaviour that a real network usually exhibits. The seed value (a non­zero positive integer)
initializes the random number generator. Different seed values will make the simulator behave slightly differently and result in different output values. You need to provide a cmd­line parameter to the simulator binary with the ­s option.																			
E.g.: $ ./abt ­s 1234

● Window size: This only applies to Go­back­N and Selective­Repeat binaries. Both these protocols use a finite­sized window to function. You need to tell the simulator	before hand, what window size you want to use. In fact, the code will internally use this value for implementing the protocols. You need to provide a cmd­line parameter to the simulator binary with the ­w option. 																									
E.g.: $ ./gbn ­s 1234 ­w 1000