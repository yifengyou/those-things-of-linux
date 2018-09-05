## Linux那些事儿之我是PCI

![1536109312199.png](assets/1536109312199.png)

![1536109373094.png](assets/1536109373094.png)

![1536109387622.png](assets/1536109387622.png)

![1536109400814.png](assets/1536109400814.png)


![1536108055927.png](assets/1536108055927.png)

![1536109410589.png](assets/1536109410589.png)



* make menuconfig就可以看到关于Bus Options的配置选项,子选项包含PCI配置，只有打开PCI support才能进入 PCI access mode(Any)子选项
* 第二项“PCI access mode”的存在，它是一个单项选择题，有四个答案， 分别是 BIOS、 MMConfig、 Direct、 Any
  * Any 选项本身就表示了你告 诉内核说前面三个答案随便一个都可以，你只要选上了它，就相当于所有的四个答案都给选上了
  * Any 就是表示你如果拿不准的话可以让内核去选择一种访 问方式
  * 内核一向都是很严谨刻板的，绝不会真的抓阄儿抓到哪个就使用哪种方式， 它会按照一定的优先级，首先尝试 MMConfig，然后是 Direct，如果这两种方式都不起效， 最后再使用 BIOS







##
