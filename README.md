1.touch message.txt
  mkdir CFY
  mv message.txt /CFY
2.cp message.txt /CFY
3.sudo apt install rsync
  mkdir empty  //创建目录empty和test
  mkdir test
  mv ~/message.txt test
  mv ~/workbench/message.txt test
  rsync --delete-before -d empty/ test/  //-delete-before接收者在传输之前进行操作，删除empty和test的文件
  rmdir empty  //删除空目录empty和test
  rmdir test

exercise 2
1.mkdir workbench 
2.touch workbench/readme.txt
3.echo -e"1\n2\n3">workbench/readme.txt
[图片]4.cat workbench/readme.txt
5.ls -a home
  command >workbench/List.txt
6.wc -m workbench/List.txt


exercise 3
1.man ls
2.man man
3.apropos calendar
  man calendar  
 

exercise 4   
1.find . -name "*.png"
2.find . -name "*hiking*" -delete 
3.mv test/*.txt data   //假设数据和照片分别以txt和陪你过格式存放于test目录中
  mv test/*.png photo
