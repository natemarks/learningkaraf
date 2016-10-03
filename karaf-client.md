#Apache Karaf client – a closer look

The Apache Karaf client is found in the bin folder of your installation. It has two intended use modes; if a command is passed to the client, it executes then exits, otherwise without a command it starts an interactive shell session. Let's look at the client's optional input, then an actual invocation:

'''

bin# client [–a port] [–h hostname] [–u username] [–p password] [–r retries] [–d retry-delay] [commands]

'''
