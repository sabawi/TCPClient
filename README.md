# TCPClient
[Linux based] Strong Encryption Communication small footprint Client for Internet of things (IofT) devices

Requires https://github.com/sabawi/TCPServer 

To build on Linux:

$ make all

This will build the project in DEBUG and RELEASE configurations as :
  ./dist/Debug/GNU-Linux/tcpclient     [Debug version] 
  ./dist/Release/GNU-Linux directories [Release version]
  
To run:

$ ./dist/Debug/GNU-Linux/tcpclient [server hostname] [server port]

If no arguments were provided, you can connect to server from the command line 'CMD/Text>'

CMD/Text>help
Local Commands:
	 !q : Exit client 
	 connect <hostname> <port number> [as alias] : Connect to remote host
	 diconnect <alias> : Disconnect from remote host
	 show connections : List active connections
	 show myname : Show client current name 
	 set myname <client name> : Set client current name

Remote Commands: 
	 get file <remote filename> : Request a file from remote host
	 run <remote sscript> : Execute remote script at the host

EXAMPLE:
To connect to server code running on 192.168.1.122 and listening on port 3490
$ ./dist/Debug/GNU-Linux/tcpclient 192.168.1.122 3490


