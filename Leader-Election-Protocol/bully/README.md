
Bully leader election algorithm implementation for distributed systems.
This project implements a Leader Election Protocol using the Bully Algorithm in Python, designed for distributed systems where nodes need to agree on a single leader. The Bully Algorithm ensures that the node with the highest ID is elected as the leader, even if some nodes fail during the process. Using ZeroMQ for communication, the project simulates a network of nodes that coordinate to elect a leader in a fault-tolerant manner. Whether you're exploring distributed systems or learning about fault-tolerant algorithms, this project provides a hands-on way to understand how nodes in a network can self-organize and recover from failures. It's a great example of how simple yet powerful algorithms can solve real-world problems in distributed computing. Feel free to dive in, test it out, and contribute!

# run

numProc is the total number of nodes, numAlive is the number of nodes that are alive - online and numStarters are the number of nodes that will initiate the protocol. Timeout is determined as num_proc + 10 seconds experimentally. After broadcast message you should wait some time in accordance with number of processes due to handling terminate messages, but eventually the program terminates.

    python bully.py numProc numProc numStarters

