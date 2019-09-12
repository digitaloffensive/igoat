Server Setup:
- spin up apache server on a virtual machine or locally.
- Copy the myapp folder and its contents to your webroot
- Make sure you can browse to http://your_server_ip/myapp/checkout/ <-- should see a message that says hi.

Setting up application
- iGoat IPA running on simulator or jailbroken devie.
- If you downlaod from the offical repo you will need to modify the code under the crypto challenge on line 32 to this:
 NSMutableURLRequest *request = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:@"http://your_ip_here/myapp/checkout.php"]
 - Or clone this fork and modify just the IP.
 - Replace iGoat.xcodeproj with the contents from iGoat.xcodeproj.zip
 
 
