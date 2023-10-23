
Types of Message Passing Interface primitives:

- MPI_bsend - append outgoing message to a local send buffer
- MPI_send - send a message and wait until copied to local or remote buffer
- MPI_ssend - send a message and wait until receipt starts
- MPI_sendrecv - send a message and wait for reply
- MPI_isend - pass reference to outgoing message and continue
- MPI_issend - pass reference to outgoing message and wait until receipt starts
- MPI_recv - receive a message; block if there's none
- MPI_irecv - check if there's an incoming message but don't block