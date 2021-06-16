# wireshark-sniffing
First, we boot ubuntu on the virtual machine.

![1](https://user-images.githubusercontent.com/78695812/122205218-ad2a7300-cea8-11eb-8ace-1e16c9d402dc.jpg)

Then we open our application with the command "sudo wireshark"

![2](https://user-images.githubusercontent.com/78695812/122205234-b0bdfa00-cea8-11eb-9df8-fefdd2f2a2eb.jpg)

Then we open the network named enp0s3 by double-clicking on it to watch. This network means wifi network in ubuntu. Here we can monitor traffic on wifi network

![3](https://user-images.githubusercontent.com/78695812/122205232-b0bdfa00-cea8-11eb-8da7-7940cc62f398.jpg)

In this monitoring process, we filter the http protocol to monitor the traffic performed with the http protocol.

![4](https://user-images.githubusercontent.com/78695812/122205231-b0256380-cea8-11eb-9840-7964d89549fc.jpg)

Then we login to http://testphp.vulnweb.com/login.php on the host After logging in, the page redirects us to http://testphp.vulnweb.com/userinfo.php.

![5](https://user-images.githubusercontent.com/78695812/122205230-b0256380-cea8-11eb-95a2-5072ce93804c.jpg)

After this process, the traffic generated via wireshark appears.
Here we will examine the post processing
There are 2 post processes.

![6](https://user-images.githubusercontent.com/78695812/122205242-b1ef2700-cea8-11eb-9ab8-5f3274cb89e1.jpg)

When we open the post traffic, when we click on the "HTML form urlencoded: " field, we can monitor all the parameters sent in the post process and the entered values at the bottom.

![7](https://user-images.githubusercontent.com/78695812/122205240-b1569080-cea8-11eb-933e-42bfcc626c3f.jpg)

The parameters and values of the second post process are also displayed.

![8](https://user-images.githubusercontent.com/78695812/122205525-01cdee00-cea9-11eb-8e52-ffab6080cd32.jpg)
