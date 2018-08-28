[View on StackOverflow ..](https://stackoverflow.com/questions/46476470/cant-create-project-on-netbeans-8-2/48535841#48535841)

I had the same problem I installed NetBeans 8.2 on macOS High Sierra, and by default settings, NetBeans will work with the latest JDK release (currently JDK 9). 

[![NetBeans Problem][1]][1]

What I did was forcing NetBeans to use JDK 8, you must config your `netbeans.conf` file, you can find it on:

>/Applications/NetBeans/NetBeans 8.2.app/Contents/Resources/NetBeans/etc/netbeans.conf

[![enter image description here][2]][2]

You need to uncomment and update your path to JDK, you will find yours at:

>/Library/Java/JavaVirtualMachines/jdk1.8.0_131.jdk/Contents/Home

[![enter image description here][3]][3]

Just save it, restart NetBeans and you are done!

  [1]: https://i.stack.imgur.com/0xq9x.gif
  [2]: https://i.stack.imgur.com/qtQle.png
  [3]: https://i.stack.imgur.com/2lCRF.png
