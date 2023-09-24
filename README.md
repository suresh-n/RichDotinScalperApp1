# RichDotinScalperApp for Shoonya

RichDotinScalperApp is created using PyQt6 and Python to increase performance and can be used with the Shoonya API for scalping in index options like Nifty, BankNifty, and FinNifty.

The RichDotinScalper App is a platform designed to help traders place orders quickly to their broker terminals without having to log in to the broker’s user interface. Here are some of the features of this tool:

- You can easily buy call and put options by selecting the strike and clicking the buy button or using keyboard shortcuts added for buy buttons.

- Once the order is triggered, you can view the order details and position details in a table.

- To exit a position, you can right-click on the position and select the “Exit Market” option or by "Exit Manual".

- You can set a stop-loss order just by right-clicking on a position and selecting the “Stop Loss” option and entering the SL and trigger price.

- Additionally, you can manually trail the stop-loss order by selecting the “Trigger Pending Order” using the trail SL option.

**New Feature:** We have added a new feature for manually trailing the stop-loss, and this time you don't need to change the price manually. Just click the "Trail 2 Points" option, which will trail your position by two points up. We've also added a keyboard shortcut for this.

### How to Set up the App

1. Download the zip file from this Git repo's release and extract it. Find `RichDotinScalperApp.exe` and run it. It's a portable app, so there's no need for installation.

![image](https://github.com/suresh-n/RichDotinScalperApp1/assets/17276643/f015c498-48ea-4304-a135-00232a6e6abd)

2. The first time you launch the app and click the login button, a credentials form will pop up. Add your credentials, API, and authenticator details.

3. Once you've entered all the details, click "Submit." These details will be added to the `config.ini` file.

4. Relaunch the app and click "Login." Now, it should be all set, and you should see "Login Success!" in the message area.

![Login Success](https://github.com/suresh-n/RichDotinScalperApp1/assets/17276643/026247e8-8b85-4d8e-a0ae-32b524d0f416)

### How to Use the Scalper App

1. Launch the app and click "Login." Once you see the "Login Success" message at the bottom of the app, you're ready to use it.

2. By default, the Weekly option is selected. Use the index or strike tool to subscribe to strike prices via WebSocket, displaying live prices on the right-hand side.

3. When you're ready to trade, click on "Cash Margin." The margin will refresh, and you can move the slider to allocate your capital. The quantity will be determined accordingly.

4. Select the order type (Limit or Market), and you're ready to click buy buttons or use shortcut keys.

5. Once you click the buy button, the order will be sent to your broker's terminal and appear in the order window with its status. When the order is executed, the position will also be displayed in the position window, including the PnL (Profit and Loss).

6. Right-click on a position to access options like "Exit Market," "Exit Manual," and "Stop Loss."

   - **Exit Market**: Exit the position with a market order.
   - **Exit Manual**: Manually exit the quantity by specifying the limit price and quantity.
   - **Stop Loss**: Set a stop loss for the position by entering the price and trigger price.

7. The order table provides three options when you right-click:

   - **Modify**: Modify your order if it's open, convert it to a market order, or execute it at the current price.
   - **Trail Order**: Trail the price or the SL order (in trigger pending state).
   - **Cancel Order**: Cancel open orders or SL orders.
   - **Trail 2 Points**: Adjust the SL price up by 2 points with a click or a shortcut key.

### Shortcut Keys 

- **Left Arrow**: Buy call button
- **Right Arrow**: Buy Put button
- **Key C**: Squre Off All or close button
- **Key T**: Trail 2 points up from price. 

There was option set for main windows always top the same not applied for sl windows,etc.. if you dont seen the option after click menu items then just move the app you can see it behind will try to correct this next release. 

### Note
Please contact your financial adviser before placing your trade. We are not responsible for any trading loss or issues that occur due to broker API problems.
