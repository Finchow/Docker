# Wordpress Server

customisable wordpress server for docker-compose.

ports used: loclahost:80:80

remember to change "localhost" to your local ip and change "passwd" to your disired password.
the port number can be changed to any port you have access to. 

run "docker-compose up -d" in the directory where the "docker-compose.yml" file is located to build the image.

the url for the website should be: http://"your_local_ip"/

to get your local ip type "ip addr" in the terminal.

and if you changed the port append: http://"your_local_ip"/:"portnumber"
(if you kept the port at 80:80 you do not need this.) 

after serching the url in your browser create your account.


to port forward alllow the port through you firewall "ufw allow 80" or "ufw allow portnumber", then allow the port on your router login to the routers settigs menu then try looking into the virtual servers tab or the port forwarding tab usually under security then allow the port you are using on both tcp and udp and select your local ip address.

people can now connect to you over the internet if they put in your external ip, to get this serch what is my ip into google and it should appear they can connect by using your external ip in their browser (if you chnged the port the url would be: externalip:portnumber).

your public ip changes every day so if you wan your website to stay up for long you will need  a domain name, be aware of hackers port 80 can be dangerous maybe invest in getting a https certificate for a more secure port.
