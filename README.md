# Prism-SkyLab-Ops-Test
Technical assessment

I installed haproxy as the software solution to redirect traffic between 2 internal servers.
I came across 2 issues I couldn't resolve.
1st issue, is I am unable to access the frontend url port 80 http://user-facing.thorton.dev.prismsl.net 
I was concerned if the security group in AWS allows http access, otherwise I would be anxious to know how to get around this.
2nd issue, after installing haproxy and using curl locally (since I couldnt check from web browser per above) I would get a 400 response from the internal servers indicating that there may be an issue with ALLOWED_HOSTS setting I believe on the django servers in the backend. I believe the issue is that I was unable to match the literal string of server names with the names presented by haproxy (per the syslog). Again I am eager to see what the resolution for this issue as well.

The uploaded tar file should include haproxy (config change to enable the service), haproxy.cfg (to enable load balancing), and syslog to validate from the machine itself that loadbalancing did occur simply from  running curl command locally on the frontend webserver.

I daresay I enjoyed this evaluation, thanks!
