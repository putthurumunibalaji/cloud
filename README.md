1.Create a text file
2.Ensure any user can read and write it
3.Compress the file using tar or zip
solution:
1.codebind@DESKTOP-N3JS6V2:~$ vi samplefile

2.codebind@DESKTOP-N3JS6V2:~$ chmod a+rw samplefile
codebind@DESKTOP-N3JS6V2:~$ stat samplefile
  File: samplefile
  Size: 53              Blocks: 0          IO Block: 4096   regular file
Device: 2h/2d   Inode: 5066549581271286  Links: 1
Access: (0666/-rw-rw-rw-)  Uid: ( 1000/codebind)   Gid: ( 1000/codebind)
Access: 2022-03-15 21:32:41.398048300 +0530
Modify: 2022-03-15 21:32:41.398048300 +0530
Change: 2022-03-15 21:33:44.872950200 +0530
 Birth: -

3.codebind@DESKTOP-N3JS6V2:~$ tar -czf samplefile.tqz samplefile
  codebind@DESKTOP-N3JS6V2:~$ ls -lh samplefile.tqz
 -rw-r--r-- 1 codebind codebind 164 Mar 15 21:35 samplefile.tqz
