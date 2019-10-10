```
 ██████╗ █████╗  ██████╗  ██████╗ █████╗  ██████╗ 
██╔════╝██╔══██╗██╔═══██╗██╔════╝██╔══██╗██╔═══██╗
██║     ███████║██║   ██║██║     ███████║██║   ██║
██║     ██╔══██║██║   ██║██║     ██╔══██║██║   ██║
╚██████╗██║  ██║╚██████╔╝╚██████╗██║  ██║╚██████╔╝
 ╚═════╝╚═╝  ╚═╝ ╚═════╝  ╚═════╝╚═╝  ╚═╝ ╚═════╝ 

```
![caocao.jpg](https://i.loli.net/2019/10/09/SmHx9ofZu8YlGEi.jpg)

| Service | Badge |
|----------|---------------------------------------------------------------------|
| **MakeAPullRequest** 	| [![Pull Requests Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat)](http://makeapullrequest.com)|
| **FirstTimersOnly** 	|[![first-timers-only Friendly](https://img.shields.io/badge/first--timers--only-friendly-blue.svg)](http://www.firsttimersonly.com/)|
| **CodeTriage** 	| [![Open Source Helpers](https://www.codetriage.com/enzo-sun/caocao/badges/users.svg)](https://www.codetriage.com/freecodecamp/freecodecamp)|
| **GitPod** 	| [![Setup Automated](https://img.shields.io/badge/setup-automated-blue?logo=gitpod)](https://gitpod.io/from-referrer/)|
| **TravisCI** 	| [![Build Status](https://travis-ci.org/enzo-sun/Caocao.svg?branch=master)](https://travis-ci.org/enzo-sun/Caocao.svg?branch=master)|
| **AppVeyor**  | [![Build status](https://ci.appveyor.com/api/projects/status/9cgkgxkc3203fm1o/branch/master?svg=true)](https://ci.appveyor.com/project/radareorg/radare2/branch/master)|
| **Coverity** 	| [![Build Status](https://scan.coverity.com/projects/19372/badge.svg)](https://scan.coverity.com/projects/enzo-sun-caocao)|
| **Infrastructure** |  [![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/741/badge)](https://bestpractices.coreinfrastructure.org/projects/741) |
| **Codecov** | [![codecov](https://codecov.io/gh/radareorg/radare2/branch/master/graph/badge.svg)](https://codecov.io/gh/radareorg/radare2)
| **Fuzzit** | [![fuzzit](https://app.fuzzit.dev/badge?org_id=2zv5qI33roZkRm0oO2Mi&target_id=YVkkS6RPVpKhSixyFWcT&branch=master)](https://app.fuzzit.dev/admin/2zv5qI33roZkRm0oO2Mi/target)


Caocao [中文页面](/Readme-zh.md)
===============

Caocao is the ....

Caocao can help you in three ways:
1.
2.
3.

Developers
---------
* Windows Build Status: <a href="https://ci.appveyor.com/project/Caocao/Caocao"><img src="https://ci.appveyor.com/api/projects/status/github/Caocao/Caocao"/></a>

* Coverity Scan Build Status: 



</a>

* Project stats: https://enzo-sun.github.io/Caocao/

Issues, bugs, requests, ideas
----------------------------------
Use the [issue](https://github.com/enzo-sun/Caocao/issues) tracker to report bugs.

Comms
----------------------------------
### Mailing Lists ###
Source Code


### Log:
`
</br>20190821: changed App/usbd_desc.c USBD_SERIALNUMBER_STRING_FS USBD_GetString((uint8_t *)usb_fs_slaver_addr_str_g, USBD_StrDesc, length);
</br>20190821: changed freertos.c add slaver id identify string & fun
</br>20190821: mcu osc startup ok 
</br>20190821: runnign status ok & slaver address set func ok
</br>20190822: usb driver not found，usb cdc error
</br>20190822: find out USBD_MAX_NUM_CONFIGURATION = 2, could overcome the difficult & need set heap as 0x600
</br>20190823: usb cdc description name test ok ,on new version mac mini, we can identify usb string description.
</br>20190823: usb communication error
</br>20190824: usb lib update ok
</br>20190824: update app_cmd_handle.cpp
</br>20190825: update app_cmd_handle.cpp & add cmd parsing fun
</br>20190826: test wtioe cmd,!!! usb bug, receive buf don;t exceed 60 chars , why not 64???
</br>20190827: stm16cp05 test ok, command parsing flow need optimal more
</br>20190827: prepare update cat9555 driver
</br>20190828: cat9555 driver build ok
</br>20190828: [bug]find out send over 52(not include 52) bit comfig 
</br>20190829: cat9555 verify error?(test a wrong test point)
</br>20190830: cat9555 test ok, update readback verify part.
</br>20190830: build si5351 driver ok & verify ok. generate 14.7459kHz clock. TEK
</br>20190830: update hw init structure
</br>20190831: fix stp16cp05 latch timing bug. & add cat9555 verify process
</br>20190831: find out adc data sample speed error, change cloak as 14.7465MHz
</br>20190831: adc sample speed config ok.test ok.

</br>20190902: find out ad7175-8 id is 0x40c4 but from datasheet,the value is 0x3cdx
</br>20190902: prepare build sample frame & include data average

</br>20190903: [bug]find out : after adc sample immediately, will be cause usb lost send data randomly.
</br>20190903: prepare average algorithm
</br>20190904: test, 4channel sample ok, but data acquire cause bug, need expand thread stack memory tomorrow

</br>20190905: complete dac cmd parsing, to be test.
</br>20190905: add hw init stp16cp05 init part

</br>20190905: [bug]ad7175 find init fail bug
</br>20190906: debug ok about ad7175
</br>20190906: debug cat9555 & si5351a ok
</br>20190906: update dac parts & rebuild hw init, dac to be test later

</br>20190906: !!! before dac60508 set,must care spi mode. !!!
</br>20190906: dac 1-3 init test ok
</br>20190906: dac to be test
</br>20190907: update adc & config temp struct
</br>20190909: dac brdcast mode fail, cmd parsing ok
</br>20190909: remove usb device description string bug
</br>20190910: remove dac brdcast mode bug
</br>20190910: prepare to add function point to overcome cmd parsing & handle structure
</br>20190911: fix func point parsing bug
</br>20190912: find out 4 ch adc sample bug, adc cnt_temp error: eg,randomly ch1=7 ch2=5 or ch16=7 ch1=5 ...   noemally is 6 as all cahnnel  
</br>20190914: find out the basic rason from rtos, none-os is normal. but need verify more to find detail reason.
</br>20190916: find out 4 ch adc sample bug: from 5.doe 5.Doe\4adc_sample_error folder.
</br>20190916: fixed 4ch sample bug,but find other bug on sample
</br>20190916: solve some problem but the error will be happen @1/17000times  couldn't find reason   C:\Users\Enzo.DESKTOP-4P3AATN\Desktop\bk\0. FW\Caocao\MDK-ARM\5.Doe\4adc_sample_error_remove_float_get
</br>20190917: find out the version mcu will be crash, need add some other log to verify.
</br>20190917: add assert fail & hardware error feedback info.
</br>20190919: demo for display
</br>20190920: send pc float value as hex type
</br>20190920: find out dac single channel set bug , buffer overflow. need to verify
</br>20190921: complete all cmd list frame
</br>20190923: lo_5 cap test ok.need test more to verify.
</br>20190924: find out external io storage bug & solve it ,complete external io read function.
</br>20190924: complete help frame.
</br>20190924: find out adc sample randomly bug may be cause by after spi mode switch  ....
</br>20190925: before system integration, backup
</br>20190925: cap test ok & unmate fail & verifying
</br>20190926: cap meas & time frame ok.
</br>20190927: all time meas ok & need verify -ing
</br>20190929: test timer all test complete , need verify more.

</br>20190929: add *state = rd_buf[4] & 0x0f; to mask adc hardwate bug. 

			0x00 STATUS REG[7:0]
			[7:7]RDY [7:7]ADC_[6:6]ERROR [5:5]CRC_ERROR [4:4]REG_ERROR [3:0]CHANNEL
			The ADC_ERROR bit in the status register flags any errors that
			occur during the conversion process. The flag is set when an overrange or underrange result is output from the ADC. The ADC
			also outputs all 0s or all 1s when an undervoltage or overvoltage
			occurs. This flag is reset only when the overvoltage or undervoltage
			is removed. It is not reset by a read of the data register.

</br>20191030: all time test ok. adc sample bug solve when mask hardware status flag.
</br>20191002: commit, just for backup.

</br>20191003-05: note update
</br>20191005: remove dac set debug log
</br>20191006: complete adc matrix read mode
</br>20191007: complete single channle adc read cmd & complete adc debug mode + bind adc status
</br>20191007: add dac read back function, need verify more.
</br>20191007: fix tim4 timer_channel_4_get_freq & timer_disconnect_time_meas  time out design
</br>20191008: fix cc disconnect + host detect 420nf voltage meas.
`
bug:
</br>adc id not match datasheet adc sample bug
</br>dac bug  gain error

----------------------------------
In Oct 2019, Enzo moved from
subversion to git hosted at GitHub
* https://github.com/enzo-sun/Caocao/

Enjoy,
		Enzo sun</br></br>
		
![we_chat.jpg](https://i.loli.net/2019/10/09/c4tlRhiD93bgknS.jpg)

#####文件夹说明：
1. Bin   
`存放bin文件 & Backup用的bin & hex文件（每次编译后会更新）`
1. Tool    
`存放系统工具`
1. Doc    
`存放相关文档`
1. Bsp   
`存放板级支持包BSP（Board Support Package）是介于硬件和驱动层程序之间的一层`     
`此处将驱动层也包含于此，直接在应用层调用`


代码规范化：
1.代码风格
2.出错处理
3.复杂度分析（用于提高性能）

>正确性、健壮性、可靠性、效率、易用性、可读性（可理解性）、可扩展性、可复用性、兼容性、可移植性等

（ 1）知错就改；
（ 2）经常温故而知新；
（ 3）坚持学习，天天向上。


例 如 不要 把 CurrentValue 写成NowValue。
标识符的长度应当符合“ min-length && max-information”原则
命名规则尽量与所采用的操作系统或开发工具的风格保持一致。

例如 Windows 应用程序的标识符通常采用“大小写”混排的方式，如 AddChild。而Unix 应用程序
的标识符通常采用“小写加下划线”的方式，如 add_child。别把这两类风格混在一起用。

变量的名字应当使用“名词”或者“形容词＋名词”。
float value;
float oldValue;
float newValue;

全局函数的名字应当使用“动词”或者“动词＋名词”（动宾词组）。
类的成员函数应当只使用“动词”，被省略掉的名词就是对象本身。
例如：
DrawBox(); // 全局函数
box->Draw(); // 类的成员函数


用正确的反义词组命名具有互斥意义的变量或相反动作的函数等。
例如：
int minValue;
int maxValue;
int SetValue(…);
int GetValue(…);

尽量避免名字中出现数字编号，如 Value1,Value2 等，除非逻辑上的
确需要编号。这是为了防止程序员偷懒，不肯为命名动脑筋而导致产生无意义的名
字（因为用数字编号最省事）。


DOE:

SPI5: 速度验证【OK】
FREERTOS_ ：AD7175-8 200ns 速度验证[ing ]
芯片替代交期：选型列表


ip:192.168.1.10 8888

####Plan
1.完成AD7175驱动以及复用问题， 模板和stl 配置
1.增加dsp库 
2.增加IO_Expander 驱动程序
3.拟增加USART1 串口DMA + IAP function
【待增加】USB IAP   USB DFU USB IAP使用标准库来完成设计，bootloader部分使用HAL Lib来完成
4.增加Log system


###待解决问题：
1.
1.fifo init bug

####Func:

1. USART1
1. GPIO


single 
/*第一个2.5为偏置电压，第二个2.5为参考电压.*/
voltage = 2.5 + value * 2.5 / 0xFFFFFF;</span>

bipolar mode

/*第一个2.5为偏置电压，第二个2.5为参考电压.*/
if(ad_id & 0x800000)
{
       voltege = 2.5 + (value^0x800000) * 2.5 / 0x7fffff;/*异或是在做补码计算*/
}
else
{
       voltage = 2.5 - ((value^0x7FFFFF) + 1) *2.5 / 0x7fffff;
}/*注意"+"的优先级高于"^"*/</span>



####Log
1.
1.
1.
1.

@rem ::直接运行fromelf.exe生成bin文件，未测试成功
@rem ::start  "../fromelf.exe --bin -o ../output/CONTROL_APP_Q_X.bin ../CONTROL_APP_Q_X.axf"
@rem ::start  ../fromelf.exe --bin -o $L@L.bin #L

@del /s /q ..\1.Bin\*_BK.bin
@rem ::清空*_BK.bin 文件

@rem ::输出结果格式为 20181027222620.bin
@rem ::如果不一致则是当前系统的日期格式不一致导致
@rem ::解决办法：修改系统的日期格式或者运行 TimeFormat.reg文件把日期格式导入注册表.
@rem ::获取当前时间字符串并赋值给变量T

@set strCurrentDate=%date:~0,4%%date:~5,2%%date:~8,2%%time:~0,2%%time:~3,2%%time:~6,2%

@echo on

@rem ::更改BIN文件下的文件名为当前日期
copy ..\Demo\*.bin 1.Bin\%strCurrentDate%_BK.bin
pause


---

！！！线程交互任务标志触发
#define RECV_PROTOCOL_SIGNAL      ( 1 << 0 )
#define SEND_PROTOCOL_SIGNAL      ( 1 << 1 )
#define REFEREE_SIGNAL            ( 1 << 2 )
/*线程间通信 利用该标志处理*/
//static void protocol_send_success_callback(void)
void protocol_send_success_callback(void)
{
  osSignalSet(adcGetTaskHandle, SEND_PROTOCOL_SIGNAL);
}


//		osEvent event;

//    event = osSignalWait(SEND_PROTOCOL_SIGNAL | RECV_PROTOCOL_SIGNAL | REFEREE_SIGNAL, osWaitForever);

//    if (event.status == osEventSignal)
//		{
//			if (event.value.signals & SEND_PROTOCOL_SIGNAL)
//      {
//				if (HAL_GPIO_ReadPin(GPIOB, GPIO_PIN_4) == GPIO_PIN_RESET && ++cnt <=64)
				{
//					protocol_send_success_callback();






	UART_Printf(&UPPER_COM_HUART, "\r\n ScanTask \r\n");
	uint32_t testNumber[6][8][4][16];//6:aPLC@50Hz 6 Samples 8:50mA & 100mA each 8 times 4:4Pcs ADC 16:16Channel
	uint32_t testNumber2[8][4][16];
	static __IO double runTime = 0.0f;
	static __IO uint32_t temp = 0, temp1 = 0;
	uint32_t x = 0, i = 0, j = 0, k = 0, l = 0;
	CPU_TS_TmrInit();
	
	
	for( i = 0;i < 6;i++)
	{
		for ( j = 0;j < 8;j++)
		{
			for ( k = 0;k < 4;k++)
			{
					for ( l = 0;l < 16;l++)
					{
						testNumber[i][j][k][l] = rand();
					}
			}
		}
	}
	for ( j = 0;j < 8;j++)
	{
		for ( k = 0;k < 4;k++)
		{
				for ( l = 0;l < 16;l++)
				{
						testNumber2[j][k][l] = 0;
				}
		}
	}
//------------------------------------TEST----------------------

//	Time test 

	for( i = 0;i < 6;i++)
	{
		for ( j = 0;j < 8;j++)
		{
			for ( k = 0;k < 4;k++)
			{
					for ( l = 0;l < 16;l++)
					{
						testNumber[i][j][k][l] = rand();
					}
			}
		}
	}
	for ( j = 0;j < 8;j++)
	{
		for ( k = 0;k < 4;k++)
		{
				for ( l = 0;l < 16;l++)
				{
						testNumber2[j][k][l] = 0;
				}
		}
	}

	for ( j = 0;j < 8;j++)
	{
		for ( k = 0;k < 4;k++)
		{
				for ( l = 0;l < 16;l++)
				{
						for( i = 0;i < 6;i++)
						{
								testNumber2[j][k][l] += testNumber[i][j][k][l];
						}	
				}
		}
	}
	//累加6次 251ns
	for ( j = 0;j < 8;j++)
	{
		for ( k = 0;k < 4;k++)
		{
				for ( l = 0;l < 16;l++)
				{
						for( i = 0;i < 6;i++)
						{
							testNumber2[j][k][l] <<= 5;
							temp = (((uint64_t)testNumber2[j][k][l]*0xAAAAAAABUL) >> 39);// Magic Number = 2^34 / 6 ;式|o|=2^n/(2^32-c(魔数))
							temp1 = testNumber2[j][k][l] /= 6;
							temp1 >>= 5;
						}	
				}
		}
	}
	
	i = 512;
	DWT_CYCCNT = (uint32_t)0u;//	MeasureTimeStart();
	do {	
		temp = testNumber2[0][0][0] << 5;
		testNumber2[0][0][0]  = ((uint64_t)testNumber2[0][0][0]*0xAAAAAAABUL) >> 39;//		testNumber2[0][0][0] /= 6 testNumber2[0][0][0] >>= 5;
	}while(--i);

	temp = DWT_CYCCNT;
	UART_Printf(&UPPER_COM_HUART,"\r\n Cnt:%d \r\n", temp);
	runTime	 = temp / 168000000.0f;//elapsed
