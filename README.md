
### 定制补班日程

支持指定补班日程的开始、结束时间和提醒时间，格式为：`订阅地址`?token=`API密钥`&compStart=`上班时分秒`&compEnd=`下班时分秒`&compAlarm=`在开始时间点提前多少分钟提醒`

例如补班时间为早上8.30到晚上8.30，提前15分钟提醒，则订阅地址为 `https://www.shuyz.com/githubfiles/china-holiday-calender/master/holidayCal.ics?token=cb429c2a-81a6-4c26-8f35-4f4bf0c84b2c&compStart=083000&compEnd=203000&compAlarm=15`

**注意:**
- 时间格式为24小时制的6位数字，个位补0，例如`8点零5分`表示为`080500`
- 最大可提前9999分钟提醒，所以提前几天也是可以的。例如`compStart`为`0800`，设定前一天早上8点提醒，则`compAlarm`为24x60=1440; 设定前一天晚上8点提醒，则`compAlarm`为12x60=720
- 补班日程可设置为全天事件，指定`compStart=*`并且`compEnd=*`即可
- 由于订阅功能需消耗服务器资源进行计算，如果影响到服务器的正常使用，则定制功能可能随时取消

定制补班日程表            |  详细信息
:-------------------------:|:-------------------------:
![](./customCompensateday1.png)  |  ![](./customCompensateday2.png)
