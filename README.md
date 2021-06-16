Video Link: https://drive.google.com/file/d/1BuvUdF_m8rXd_-kusYcgHUxH8hX_D9Uv/view

First, we boot ubuntu on the virtual machine.
![1](https://user-images.githubusercontent.com/78695812/122207944-612cfd80-ceab-11eb-8a56-f05d9c76bc0c.jpg)
Then we open our application with the command "sudo wireshark"

![2](https://user-images.githubusercontent.com/78695812/122207950-61c59400-ceab-11eb-846b-5a1f00764bf3.jpg)

Then we open the network named enp0s3 by double-clicking on it to watch. This network means wifi network in ubuntu. Here we can monitor traffic on wifi network
![3](https://user-images.githubusercontent.com/78695812/122207951-625e2a80-ceab-11eb-928f-1cb352291794.jpg)

In this monitoring process, we filter the http protocol to monitor the traffic performed with the http protocol.
![4](https://user-images.githubusercontent.com/78695812/122207952-625e2a80-ceab-11eb-94f2-248add0b3622.jpg)
Then we login to http://testphp.vulnweb.com/login.php on the host After logging in, the page redirects us to http://testphp.vulnweb.com/userinfo.php.
![5](https://user-images.githubusercontent.com/78695812/122207955-625e2a80-ceab-11eb-83ce-22c5541e7042.jpg)
After this process, the traffic generated via wireshark appears.
Here we will examine the post processing
There are 2 post processes.
![6](https://user-images.githubusercontent.com/78695812/122207957-62f6c100-ceab-11eb-870d-1c9c66c2a24e.jpg)
When we open the post traffic, when we click on the "HTML form urlencoded: " field, we can monitor all the parameters sent in the post process and the entered values at the bottom.
![7](https://user-images.githubusercontent.com/78695812/122207959-62f6c100-ceab-11eb-90de-b6a51682522f.jpg)
The parameters and values of the second post process are also displayed.
![8](https://user-images.githubusercontent.com/78695812/122207961-638f5780-ceab-11eb-8a6e-6ac6741ae722.jpg)
