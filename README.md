# Wingman_Cracked_1.0.6
Wingman- Toolkit for XSS Attacking. Allows you to find PoC on the site, as well as engage in crawl, and can also work in conjunction with Burp Suite. To start, you can use the -u flag if you have one domain or the -l flag list.txt if you have a list of domains, we will prescribe for the start:
![image](https://user-images.githubusercontent.com/108927927/193808974-be36a484-586f-4e2f-9c3a-9f9351f72455.png)
In the --exclude flag, we can add a few more variations, such as; dom, path, query, body. If you want to make scanning more active and efficient, then be sure to add 2 flags, these are --crawl and --progress.
Launch a Chrome session by specifying the --chrome flag. Optionally this can be combined with the -u flag to launch a window and immediately navigate to given URL.

    wingman -u http://testphp.vulnweb.com --chrome

![image](https://user-images.githubusercontent.com/108927927/193809076-36b9585d-2f6f-4d5b-b8c7-4edcf4ee5677.png)
We can also use wingman together with Burp Suite and its proxy. To do this, open the Burp Suite and go to the Proxy tab, and note HTTP History and we will display all wingman attacks

    wingman -crawl -progress -u http://testphp.vulnweb.com/ --exclude dom,path --proxy http://localhost:8080/

![image](https://user-images.githubusercontent.com/108927927/193809113-a787536b-a2be-4c2d-abb0-1aed33794453.png)
