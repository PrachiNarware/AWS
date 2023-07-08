   ,     #_
   ~\_  ####_        Amazon Linux 2023
  ~~  \_#####\
  ~~     \###|
  ~~       \#/ ___   https://aws.amazon.com/linux/amazon-linux-2023
   ~~       V~' '->
    ~~~         /
      ~~._.   _/
         _/ _/
       _/m/'
[ec2-user@ip-172-31-32-137 ~]$ sudo su -
[root@ip-172-31-32-137 ~]# yum update -y
Last metadata expiration check: 0:08:32 ago on Sat Jul  8 06:05:06 2023.
Dependencies resolved.
Nothing to do.
Complete!
[root@ip-172-31-32-137 ~]# yum install -y httpd
Last metadata expiration check: 0:09:23 ago on Sat Jul  8 06:05:06 2023.
Dependencies resolved.
===========================================================================================================================================================================================================
 Package                                              Architecture                            Version                                                   Repository                                    Size
===========================================================================================================================================================================================================
Installing:
 httpd                                                x86_64                                  2.4.56-1.amzn2023                                         amazonlinux                                   48 k
Installing dependencies:
 apr                                                  x86_64                                  1.7.2-2.amzn2023.0.2                                      amazonlinux                                  129 k
 apr-util                                             x86_64                                  1.6.3-1.amzn2023.0.1                                      amazonlinux                                   98 k
 generic-logos-httpd                                  noarch                                  18.0.0-12.amzn2023.0.3                                    amazonlinux                                   19 k
 httpd-core                                           x86_64                                  2.4.56-1.amzn2023                                         amazonlinux                                  1.4 M
 httpd-filesystem                                     noarch                                  2.4.56-1.amzn2023                                         amazonlinux                                   15 k
 httpd-tools                                          x86_64                                  2.4.56-1.amzn2023                                         amazonlinux                                   82 k
 libbrotli                                            x86_64                                  1.0.9-4.amzn2023.0.2                                      amazonlinux                                  315 k
 mailcap                                              noarch                                  2.1.49-3.amzn2023.0.3                                     amazonlinux                                   33 k
Installing weak dependencies:
 apr-util-openssl                                     x86_64                                  1.6.3-1.amzn2023.0.1                                      amazonlinux                                   17 k
 mod_http2                                            x86_64                                  2.0.11-2.amzn2023                                         amazonlinux                                  150 k
 mod_lua                                              x86_64                                  2.4.56-1.amzn2023                                         amazonlinux                                   62 k

Transaction Summary
===========================================================================================================================================================================================================
Install  12 Packages

Total download size: 2.3 M
Installed size: 6.9 M
Downloading Packages:
(1/12): apr-util-openssl-1.6.3-1.amzn2023.0.1.x86_64.rpm                                                                                                                   285 kB/s |  17 kB     00:00    
(2/12): libbrotli-1.0.9-4.amzn2023.0.2.x86_64.rpm                                                                                                                          3.8 MB/s | 315 kB     00:00    
(3/12): httpd-core-2.4.56-1.amzn2023.x86_64.rpm                                                                                                                             14 MB/s | 1.4 MB     00:00    
(4/12): httpd-tools-2.4.56-1.amzn2023.x86_64.rpm                                                                                                                           2.0 MB/s |  82 kB     00:00    
(5/12): apr-1.7.2-2.amzn2023.0.2.x86_64.rpm                                                                                                                                5.7 MB/s | 129 kB     00:00    
(6/12): mod_lua-2.4.56-1.amzn2023.x86_64.rpm                                                                                                                               4.4 MB/s |  62 kB     00:00    
(7/12): apr-util-1.6.3-1.amzn2023.0.1.x86_64.rpm                                                                                                                           4.9 MB/s |  98 kB     00:00    
(8/12): httpd-2.4.56-1.amzn2023.x86_64.rpm                                                                                                                                 1.7 MB/s |  48 kB     00:00    
(9/12): mod_http2-2.0.11-2.amzn2023.x86_64.rpm                                                                                                                             8.0 MB/s | 150 kB     00:00    
(10/12): mailcap-2.1.49-3.amzn2023.0.3.noarch.rpm                                                                                                                          2.3 MB/s |  33 kB     00:00    
(11/12): httpd-filesystem-2.4.56-1.amzn2023.noarch.rpm                                                                                                                     1.2 MB/s |  15 kB     00:00    
(12/12): generic-logos-httpd-18.0.0-12.amzn2023.0.3.noarch.rpm                                                                                                             1.6 MB/s |  19 kB     00:00    
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Total                                                                                                                                                                       12 MB/s | 2.3 MB     00:00     
Running transaction check
Transaction check succeeded.
Running transaction test
Transaction test succeeded.
Running transaction
  Preparing        :                                                                                                                                                                                   1/1 
  Installing       : apr-1.7.2-2.amzn2023.0.2.x86_64                                                                                                                                                  1/12 
  Installing       : apr-util-1.6.3-1.amzn2023.0.1.x86_64                                                                                                                                             2/12 
  Installing       : apr-util-openssl-1.6.3-1.amzn2023.0.1.x86_64                                                                                                                                     3/12 
  Installing       : mailcap-2.1.49-3.amzn2023.0.3.noarch                                                                                                                                             4/12 
  Installing       : httpd-tools-2.4.56-1.amzn2023.x86_64                                                                                                                                             5/12 
  Installing       : generic-logos-httpd-18.0.0-12.amzn2023.0.3.noarch                                                                                                                                6/12 
  Running scriptlet: httpd-filesystem-2.4.56-1.amzn2023.noarch                                                                                                                                        7/12 
  Installing       : httpd-filesystem-2.4.56-1.amzn2023.noarch                                                                                                                                        7/12 
  Installing       : httpd-core-2.4.56-1.amzn2023.x86_64                                                                                                                                              8/12 
  Installing       : mod_lua-2.4.56-1.amzn2023.x86_64                                                                                                                                                 9/12 
  Installing       : mod_http2-2.0.11-2.amzn2023.x86_64                                                                                                                                              10/12 
  Installing       : libbrotli-1.0.9-4.amzn2023.0.2.x86_64                                                                                                                                           11/12 
  Installing       : httpd-2.4.56-1.amzn2023.x86_64                                                                                                                                                  12/12 
  Running scriptlet: httpd-2.4.56-1.amzn2023.x86_64                                                                                                                                                  12/12 
  Verifying        : libbrotli-1.0.9-4.amzn2023.0.2.x86_64                                                                                                                                            1/12 
  Verifying        : apr-util-openssl-1.6.3-1.amzn2023.0.1.x86_64                                                                                                                                     2/12 
  Verifying        : httpd-core-2.4.56-1.amzn2023.x86_64                                                                                                                                              3/12 
  Verifying        : httpd-tools-2.4.56-1.amzn2023.x86_64                                                                                                                                             4/12 
  Verifying        : apr-1.7.2-2.amzn2023.0.2.x86_64                                                                                                                                                  5/12 
  Verifying        : mod_lua-2.4.56-1.amzn2023.x86_64                                                                                                                                                 6/12 
  Verifying        : httpd-2.4.56-1.amzn2023.x86_64                                                                                                                                                   7/12 
  Verifying        : apr-util-1.6.3-1.amzn2023.0.1.x86_64                                                                                                                                             8/12 
  Verifying        : mod_http2-2.0.11-2.amzn2023.x86_64                                                                                                                                               9/12 
  Verifying        : mailcap-2.1.49-3.amzn2023.0.3.noarch                                                                                                                                            10/12 
  Verifying        : httpd-filesystem-2.4.56-1.amzn2023.noarch                                                                                                                                       11/12 
  Verifying        : generic-logos-httpd-18.0.0-12.amzn2023.0.3.noarch                                                                                                                               12/12 

Installed:
  apr-1.7.2-2.amzn2023.0.2.x86_64               apr-util-1.6.3-1.amzn2023.0.1.x86_64         apr-util-openssl-1.6.3-1.amzn2023.0.1.x86_64         generic-logos-httpd-18.0.0-12.amzn2023.0.3.noarch        
  httpd-2.4.56-1.amzn2023.x86_64                httpd-core-2.4.56-1.amzn2023.x86_64          httpd-filesystem-2.4.56-1.amzn2023.noarch            httpd-tools-2.4.56-1.amzn2023.x86_64                     
  libbrotli-1.0.9-4.amzn2023.0.2.x86_64         mailcap-2.1.49-3.amzn2023.0.3.noarch         mod_http2-2.0.11-2.amzn2023.x86_64                   mod_lua-2.4.56-1.amzn2023.x86_64                         

Complete!
[root@ip-172-31-32-137 ~]# systemctl status httpd
○ httpd.service - The Apache HTTP Server
     Loaded: loaded (/usr/lib/systemd/system/httpd.service; disabled; preset: disabled)
     Active: inactive (dead)
       Docs: man:httpd.service(8)
[root@ip-172-31-32-137 ~]# mkdir temp
[root@ip-172-31-32-137 ~]# cd temp/
[root@ip-172-31-32-137 temp]# wget https://www.free-css.com/assets/files/free-css-templates/download/page292/yogast.zip
--2023-07-08 06:20:47--  https://www.free-css.com/assets/files/free-css-templates/download/page292/yogast.zip
Resolving www.free-css.com (www.free-css.com)... 217.160.0.242, 2001:8d8:100f:f000::28f
Connecting to www.free-css.com (www.free-css.com)|217.160.0.242|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 5471119 (5.2M) [application/zip]
Saving to: ‘yogast.zip’

yogast.zip                                         100%[===============================================================================================================>]   5.22M  3.87MB/s    in 1.3s    

2023-07-08 06:20:49 (3.87 MB/s) - ‘yogast.zip’ saved [5471119/5471119]

[root@ip-172-31-32-137 temp]# ls -lrt
total 5344
-rw-r--r--. 1 root root 5471119 Aug 20  2021 yogast.zip
[root@ip-172-31-32-137 temp]# unzip yogast.zip
Archive:  yogast.zip
  inflating: yogast-html/about.html  
  inflating: yogast-html/contact.html  
   creating: yogast-html/css/
  inflating: yogast-html/css/.DS_Store  
  inflating: yogast-html/css/bootstrap.css  
  inflating: yogast-html/css/bootstrap.min.css  
  inflating: yogast-html/css/font-awesome.min.css  
  inflating: yogast-html/css/jquery.mCustomScrollbar.min.css  
  inflating: yogast-html/css/owl.carousel.css  
  inflating: yogast-html/css/owl.carousel.min.css  
  inflating: yogast-html/css/owl.theme.default.min.css  
  inflating: yogast-html/css/responsive.css  
  inflating: yogast-html/css/style.css  
   creating: yogast-html/fonts/
  inflating: yogast-html/fonts/FontAwesome.otf  
  inflating: yogast-html/fonts/fontawesome-webfont.eot  
  inflating: yogast-html/fonts/fontawesome-webfont.svg  
  inflating: yogast-html/fonts/fontawesome-webfont.ttf  
  inflating: yogast-html/fonts/fontawesome-webfont.woff  
  inflating: yogast-html/fonts/fontawesome-webfont.woff2  
  inflating: yogast-html/fonts/IcoMoon-Free.ttf  
  inflating: yogast-html/fonts/Poppins-Black.ttf  
  inflating: yogast-html/fonts/Poppins-BlackItalic.ttf  
  inflating: yogast-html/fonts/Poppins-Bold.ttf  
  inflating: yogast-html/fonts/Poppins-BoldItalic.ttf  
  inflating: yogast-html/fonts/Poppins-ExtraBold.ttf  
  inflating: yogast-html/fonts/Poppins-ExtraBoldItalic.ttf  
  inflating: yogast-html/fonts/Poppins-ExtraLight.ttf  
  inflating: yogast-html/fonts/Poppins-ExtraLightItalic.ttf  
  inflating: yogast-html/fonts/Poppins-Italic.ttf  
  inflating: yogast-html/fonts/Poppins-Light.ttf  
  inflating: yogast-html/fonts/Poppins-LightItalic.ttf  
  inflating: yogast-html/fonts/Poppins-Medium.ttf  
  inflating: yogast-html/fonts/Poppins-MediumItalic.ttf  
  inflating: yogast-html/fonts/Poppins-Regular.ttf  
  inflating: yogast-html/fonts/Poppins-SemiBold.ttf  
  inflating: yogast-html/fonts/Poppins-SemiBoldItalic.ttf  
  inflating: yogast-html/fonts/Poppins-Thin.ttf  
  inflating: yogast-html/fonts/Poppins-ThinItalic.ttf  
  inflating: yogast-html/games.html  
   creating: yogast-html/icon/
   creating: yogast-html/images/
  inflating: yogast-html/images/.DS_Store  
  inflating: yogast-html/images/about_btn.png  
  inflating: yogast-html/images/about_img.png  
  inflating: yogast-html/images/banner1.jpg  
  inflating: yogast-html/images/bbnner.png  
  inflating: yogast-html/images/bg-body.jpg  
  inflating: yogast-html/images/call.png  
  inflating: yogast-html/images/clint.jpg  
  inflating: yogast-html/images/foot.png  
  inflating: yogast-html/images/footer_bg.png  
  inflating: yogast-html/images/loading.gif  
  inflating: yogast-html/images/logo.png  
  inflating: yogast-html/images/mall.png  
  inflating: yogast-html/images/menu_btn.png  
  inflating: yogast-html/images/sport1.png  
  inflating: yogast-html/images/sport2.png  
  inflating: yogast-html/images/sport3.png  
  inflating: yogast-html/index.html  
   creating: yogast-html/js/
  inflating: yogast-html/js/.DS_Store  
  inflating: yogast-html/js/bootstrap.bundle.min.js  
  inflating: yogast-html/js/bootstrap.js  
  inflating: yogast-html/js/bootstrap.min.js  
  inflating: yogast-html/js/custom.js  
  inflating: yogast-html/js/jquery.mCustomScrollbar.concat.min.js  
  inflating: yogast-html/js/jquery.min.js  
  inflating: yogast-html/js/jquery-3.0.0.min.js  
  inflating: yogast-html/js/owl.carousel.js  
  inflating: yogast-html/js/owl.carousel.min.js  
  inflating: yogast-html/tranner.html  
[root@ip-172-31-32-137 temp]# ls -lrt
total 5344
-rw-r--r--. 1 root root 5471119 Aug 20  2021 yogast.zip
drwxr-xr-x. 7 root root     160 Jul  8 06:22 yogast-html
[root@ip-172-31-32-137 temp]# cd yogast-html
[root@ip-172-31-32-137 yogast-html]# ls -lrt
total 124
drwxr-xr-x. 2 root root     6 Jul 27  2019 icon
-rw-r--r--. 1 root root 11223 Feb 28  2020 tranner.html
-rw-r--r--. 1 root root 19802 Feb 28  2020 index.html
-rw-r--r--. 1 root root  8270 Feb 28  2020 games.html
-rw-r--r--. 1 root root  7216 Feb 28  2020 contact.html
-rw-r--r--. 1 root root  6413 Feb 28  2020 about.html
drwxr-xr-x. 2 root root 16384 Apr 27  2020 js
drwxr-xr-x. 2 root root 16384 Apr 27  2020 images
drwxr-xr-x. 2 root root 16384 Apr 27  2020 fonts
drwxr-xr-x. 2 root root 16384 Apr 27  2020 css
[root@ip-172-31-32-137 yogast-html]# mv * /var/www/html
[root@ip-172-31-32-137 yogast-html]# cd /var/www/html
[root@ip-172-31-32-137 html]# ls -lrt
total 124
drwxr-xr-x. 2 root root     6 Jul 27  2019 icon
-rw-r--r--. 1 root root 11223 Feb 28  2020 tranner.html
-rw-r--r--. 1 root root 19802 Feb 28  2020 index.html
-rw-r--r--. 1 root root  8270 Feb 28  2020 games.html
-rw-r--r--. 1 root root  7216 Feb 28  2020 contact.html
-rw-r--r--. 1 root root  6413 Feb 28  2020 about.html
drwxr-xr-x. 2 root root 16384 Apr 27  2020 js
drwxr-xr-x. 2 root root 16384 Apr 27  2020 images
drwxr-xr-x. 2 root root 16384 Apr 27  2020 fonts
drwxr-xr-x. 2 root root 16384 Apr 27  2020 css
[root@ip-172-31-32-137 html]# systemctl status httpd
○ httpd.service - The Apache HTTP Server
     Loaded: loaded (/usr/lib/systemd/system/httpd.service; disabled; preset: disabled)
     Active: inactive (dead)
       Docs: man:httpd.service(8)
[root@ip-172-31-32-137 html]# systemctl enable httpd
Created symlink /etc/systemd/system/multi-user.target.wants/httpd.service → /usr/lib/systemd/system/httpd.service.
[root@ip-172-31-32-137 html]# systemctl start httpd
[root@ip-172-31-32-137 html]# systemctl status httpd
● httpd.service - The Apache HTTP Server
     Loaded: loaded (/usr/lib/systemd/system/httpd.service; enabled; preset: disabled)
     Active: active (running) since Sat 2023-07-08 06:38:23 UTC; 4s ago
       Docs: man:httpd.service(8)
   Main PID: 26606 (httpd)
     Status: "Started, listening on: port 80"
      Tasks: 177 (limit: 1114)
     Memory: 12.8M
        CPU: 70ms
     CGroup: /system.slice/httpd.service
             ├─26606 /usr/sbin/httpd -DFOREGROUND
             ├─26607 /usr/sbin/httpd -DFOREGROUND
             ├─26608 /usr/sbin/httpd -DFOREGROUND
             ├─26609 /usr/sbin/httpd -DFOREGROUND
             └─26610 /usr/sbin/httpd -DFOREGROUND

Jul 08 06:38:23 ip-172-31-32-137.ap-south-1.compute.internal systemd[1]: Starting httpd.service - The Apache HTTP Server...
Jul 08 06:38:23 ip-172-31-32-137.ap-south-1.compute.internal systemd[1]: Started httpd.service - The Apache HTTP Server.
Jul 08 06:38:23 ip-172-31-32-137.ap-south-1.compute.internal httpd[26606]: Server configured, listening on: port 80
[root@ip-172-31-32-137 html]#
