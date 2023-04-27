# RichDotinScalperApp for Shoonya

RichDotinScalperApp is created using PyQt6 and python to increase the performance and can be used with Shoonya API for scalping in index option Nifty/BankNifty.

The RichDotinScalper App is a platform designed to help traders place orders quickly to their broker terminals without having to login to the broker’s user interface. Here are some of the features of this tool:

You can easily buy call and put options by selecting the strike and clicking the buy button.

Once the order is triggered, you can view the order details and position details in a table.

To exit a position, you can right-click on the position and select the “Exit Market” option.

You can set a stop-loss order by right-clicking on a position and selecting the “Stop Loss” option.

Additionally, you can manually trail the stop-loss order by selecting the “Trigger Pending Order” using trail SL option.

``
#### How to setup the App

Downloaed the zip file in this git repo and extract it, then find the RichDotinScalperApp.exe and run it. It's kind of portable App no need of any installation. 

* First time when you launch, when you click login button the credentials form pops up, we just need to add credential, API and authenticator details.

![](https://i.imgur.com/mYmgv2s.png)

* Once all the details entered just click submit! you're done. The details added here will be added to config.ini file.
* Relaunch the App and click Login now it should be all set. Should show Login Sucess! in msg area.

![](https://i.imgur.com/mKlUnt9.png)


#### How to Use the Scalper App 
* Launch the App and click Login, Once you login sucess msg in bottom of the app you're ready.
* Now by defauly the Weekly option is selected, just the index or strike tool will subscribe those strike in websocket and showcase the live price in right hand side. 
* when you're ready for taking a trade just click on cash margin and the margin will be refreshed the move the slider how much capital use want tp use accordingly the qty qill be decided. 
* Select order type Limit or marker, now you're reay to click buy buttons. 
* ok, once you click buy button the orer will be send to broker terminal and show up in order windows with status, if the order is completed the position also shown in position windows dislying pnl.
* Now when you Right click on the position you can see option like "ExitMkt" "Exit Manual" "Stoploss"
 
> **Exit Mkt  We can just exit the position with market order by clicking this option**

> **Exit Manual  We can just manually exit the qty byadding the limit price and qty.**
> 
> **Stopploss We can set stop loss of the position just by entering the price and trigger price.**

* The order table will show all the orders and when you right click there are 3 options 
> **Modify This will modify your order if its open and set to market order or make it hit at current price.** 

> **Trail Order Using this we can trail the price or the SL order[which is in trigger pending state]**

> **Cancel Order We can cancel the open order or SL orders**

#### Note:
Please contact your financial adviser before placing your trade. We are not responsible for any trading loss or broker api errors.
