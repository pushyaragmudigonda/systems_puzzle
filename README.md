## Changes made:-

1) The port number 5001 exposed in dockerfile, but the same is not updated in app.py 
   I Have Made the necessary changes by initializ port no 5001 in app.py
   app.run(host='0.0.0.0', port=int("5001"))

2) In the "docker-compose.yml", the flask app is listening on port no 80 according to flaskapp.conf.  The port number was not in order in the yml file. Changed the ports accordingly.
    "8080:80"
    
3) In the yml file, local folder where the data need to be stored is specified incorrect.
   "data" -> "./data"
   

