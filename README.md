# 用于评价生成图片的选图评分器
### choose-the-better-picture
A score application to verify pictures generated by different methods</br>

#### 使用说明：



</br>；

#### 修改记录：

**2019/02/02 KaLuLas**

**修改(poll.py)：**

新增限制：工程文件夹和方法文件夹中不能包含“.”符号

修改了保存 / 不保存退出的UI，现使用messagebox

现在可以选择工程文件夹和存放原始图像的文件夹

对存档results.txt文件做了修改

TODO：选择文件夹可以用filedialog模块实现，设计可能会不太一样

TODO：评分结束后的确认保存

TODO：看看能不能让窗口不那么闪

</br>

**2019/01/31 KaLuLas**

**修改(poll.py)：**

- [x] 读取路径修改，修改为相对路径

- [x] 选择工程文件夹，选择原始图像文件夹

- [x] *使用限制：对应方法的图片文件名至少以“_method”的方式包含该方法名

- [x] 修改了得到图片文件名的方法

- [x] 在GUI中显示当前的评分进度

- [x] 保存的退出和不保存的退出

- [x] 显示方法总数和图片总数的listbox：

  在选图界面显示当前项目有几种生成方法，“原始图像”文件夹下有几张图片

- [x] 点击按钮触发窗口，显示当前工程下的评分结果

- [x] 可显示当前图片生成方法的按钮（测试用

  触发按钮时会在左右图上打上label显示这是由哪种方法生成的

- [x] 显示原始图片文件名

  最左边的原始图片栏打上label显示文件名

- [ ] 断点续评（pickle？

- [x] 结果保存文件里看不出哪个是哪个

  现在result.txt里面看不出来各个得分是哪个生成方法的，保存格式可能得修改一下

- [ ] 存在图片文件格式问题

- [ ] 自定义选图提示