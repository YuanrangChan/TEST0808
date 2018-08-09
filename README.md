# PBOSS_MakeCardData_AutoTest

项目背景：
   项目上的卡资源申请需要发报文生成订单，多次加密上传文件并报文反馈，流程相当繁琐耗时，本项目旨在实现一键完成所有流程，包括报文生成发送，文件生成加密上传反馈报文，以及最终下发的卡资源及索引文件的下载。

更新记录：
2018-08-05 
 立项。完成握奇生成数据部分编码。

2018-08-06 
 创建woqi-wcpcarddata库,首次上传制卡部分代码，主要是实现随机或者按照用户输入模拟生成握奇卡数据及秘钥索引文件。
 
2018-08-07 
 实现并增加随机或者按照用户输入模拟生成写卡平台卡数据及秘钥索引文件。

2018-08-08 
   基本实现一键完成所有流程(MakeCardDataApply.py)，包括报文生成发送，文件生成加密上传反馈报文，以及最终下发的卡资源及索引文件的下载。部分数据采用交互模式来获取用户输入，可以实现不同省及号段等相关信息的灵活化。IMSI，ICCID，EID目前也是采用交互模式，由用户自行输入，后续将优化为Python连接Linux从日志中直接获取。

2017-08-09 
   优化代码(MakeCardDataApply_new.py)，IMSI，ICCID，EID不再采用交互模式，已实现Python连接Linux从日志中直接获取。至此，除制卡订单需要去CSP前台审核以外，其余流程基本实现自动化，无需人工干预。还可以优化的部分：直连DDS或分省判断连接数据库查询订单状态以更稳定更高效地把控整个流程变化。

