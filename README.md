# PBOSS_MakeCardData_AutoTest
  项目上的卡资源申请需要发报文生成订单，多次加密上传文件并报文反馈，流程相当繁琐耗时，本项目基本可以实现一键完成所有流程，包括报文生成发送，文件生成加密上传反馈报文，以及最终下发的卡资源及索引文件的下载。
  部分数据采用交互模式来获取用户输入，可以实现不同省及号段等相关信息的灵活化。IMSI，ICCID，EID目前也是采用交互模式，由用户自行输入，后续将优化为Python连接Linux从日志中直接获取。
