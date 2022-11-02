
Using fork and multi-threading has different use cases.

**1. fork()

fork is one of a few mechanisms to create a new process in Linux.
other alternatives are
system() -- Inefficient and risky
vfork() -- similar to fork but doesn't create identical copy of parent address
space, you have to call exec or exit immediately in child.
Now coming to fork(), it creates a new child process and creates a new address space identical to parent.
So whenever you run any program in your shell it calls fork() and then executes your binary in that new child process, because to create a new process it has to be child of some process, that is how Linux works.

When we want to run any unrelated programs we use fork and run the unrelated binary in new child process and now that's a separate process.

**2. Multi-threading.

In simple words in a single program , if we want to perform multiple task in parallel we use multi-threading.
Taking an example of some ticket booking server. You have multiple tickets(shared resource) available, we have a socket listening for incoming connections from client , as soon a connection is established we can create a new thread to handle that request, In the mean time original thread will continue to listen for new connection and so on. Here you have one program and one related resource, so here fork() doesn't make sense. Multithreading is useful in these kind of situations.
