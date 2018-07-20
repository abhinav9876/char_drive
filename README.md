# char_drive is a device driver module for virtual device which can be open, read and close only by any process

<h4>TO compile and clean the module</h4>
<ul>
  <li># make
    <li># make clean
  </ul>
<h4>To install amd remove module from kernel</h4>
<ul>
  <li># insmod chardev.ko
    <li># rmmod chardev.ko
 </ul>
 
 <h4> Make use of driver make device file in /dev using mkmod command with major number which will generate randomly so check your log msg for that. To try driver use:</h4>
  <ul>
  <li># cat /dev/chardev_file // let "chardev_file" we create using mkmod
  </ul>
  
<h4>It can also be use as file (special file) in program in any programming language with open, read and close statement.</h4>
