# GDPR_report_select_V1.2
 根据GDPR安全筛选跨境传输或者非加密的数据

GDPR报告数据筛选工具使用说明:

时间：  2020.04.10（创建）

2020.04.11（修改）

2020.06.06（修改）

 

 

\1.   打开\dist下的config.ini文件，path为待分析报告所在绝对路径，white_path为白名单表的绝对路径；

![img](file:///C:/Users/XIAOCU~1.ZHE/AppData/Local/Temp/msohtmlclip1/01/clip_image002.jpg)

![img](file:///C:/Users/XIAOCU~1.ZHE/AppData/Local/Temp/msohtmlclip1/01/clip_image004.jpg)

备注：path的文件应该是.xlsx，path和white_path下的数据必须为报告和白名单的完整绝对路径，且待分析的报告的sheet表名称为“全部数据”（excel模版放在test_file下），必须是.xlsx后缀文件。**（备注：如果不是.xlsx文件，则把文件另存为.xlsx格式）**

 

\2.   检查完数据后执行\dist下的GDPR_select.exe，执行脚本需要选择EU或者AU，根据实际情况选择即可，执行脚本过程中日志不断打印，执行完则自动关闭运行窗口；

 

备注：  EU筛选出非安全传输的数据和跨境传输数据

​         	 AU筛选出非安全传输的数据

![img](file:///C:/Users/XIAOCU~1.ZHE/AppData/Local/Temp/msohtmlclip1/01/clip_image006.jpg)

![img](file:///C:/Users/XIAOCU~1.ZHE/AppData/Local/Temp/msohtmlclip1/01/clip_image008.jpg)

 

\3.   执行完脚本后，检查报告：

EU生成的sheet“非欧盟国家跨境传输数据”和sheet“HTTP传输数据”为最终需要确认发出来的数据，如图1；

AU则生成sheet“非安全传输数据”，如图2；

![img](file:///C:/Users/XIAOCU~1.ZHE/AppData/Local/Temp/msohtmlclip1/01/clip_image010.jpg)

​                                                      图1

![img](file:///C:/Users/XIAOCU~1.ZHE/AppData/Local/Temp/msohtmlclip1/01/clip_image012.jpg)

​                                                    图2