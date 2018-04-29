# IpfsIosAppExample
Example Ipfs app for iOS. Requires an https proxy.


## Install

For MAC OS :

1. Install  carthage

    $ brew install carthage 

2. update frameworks for ios 

	$carthage update --platform iOS

3. check if the IPFSApi framewoeks installed in Xcode at the "Build Phases"
  
4. Install "ngrok" ,flow these [steps](https://ngrok.com/download)
    
5. Run IPFS daemon on your local OS.
     
    $ ipfs  daemon 

        Initializing daemon...
        Successfully raised file descriptor limit to 2048.
        Swarm is limited to private network of peers with the swarm key
        Swarm key fingerprint: xxx
        Swarm listening on /ip4/127.0.0.1/tcp/4001
        Swarm listening on /ip4/169.254.52.146/tcp/4001
        Swarm listening on /ip4/192.168.2.161/tcp/4001
        Swarm announcing /ip6/::1/tcp/4001
        API server listening on /ip4/127.0.0.1/tcp/5001
        Gateway (readonly) server listening on /ip4/127.0.0.1/tcp/8080
        Daemon is ready
      
6. Run ngrok proxy 
  
	$ ngrok http  5001
    
    Session Status                online                                                                           
      Account                       chaim (Plan: Free)                                                               
      Version                       2.2.8                                                                            
      Region                        United States (us)                                                               
      Web Interface                 http://127.0.0.1:4040                                                            
      Forwarding                    http://d79c1a28.ngrok.io -> localhost:5001                                       
      Forwarding                    https://d79c1a28.ngrok.io -> localhost:5001                                      

      Connections                   ttl     opn     rt1     rt5     p50     p90                                      
                                    0       0       0.00    0.00    0.00    0.00

