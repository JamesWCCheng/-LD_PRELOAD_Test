# LD_PRELOAD Tester

讓原本執行檔呼叫的function, 透過這方式去hook讓他走其他同名的實作
$ make
$ LD_PRELOAD=./lib/libhooker.so ./main

原本應該走的是libdyn2dyn, 卻被你這樣hook到 libhooker.so裡面同名的function

Cool
