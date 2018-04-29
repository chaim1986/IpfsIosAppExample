# IpfsIosAppExample
Example Ipfs app for iOS. Requires an https proxy.


## Install

For MAC OS :

  1. Install  carthage 

    $ brew install carthage 

  2. update frameworks for ios 

    $carthage update --platform iOS

  3. check if the IPFSApi framewoeks installed in Xcode at the "Build Phases"
  
  
  4. Install "ngrok"
  
    flow this steps: https://ngrok.com/download
    
  5. Run ngrok proxy 
  
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

 6. Run IPFS daemon on your local OS.
     
     $ ipfs  daemon 
   


