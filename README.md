# RichDotinScalperApp for Shoonya and Flattrade

RichDotinScalperApp is created using PyQt6 and Python to increase performance and can be used with the Shoonya and Flattrade API for scalping in index options like Nifty, BankNifty, and FinNifty.

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

2. The first time you launch the app and click the login button, a credentials form will pop up. Add your credentials, API, and authenticator details. [For Flattrade we need to manually enter the required login details in cred.yml file]

3. Once you've entered all the details, click "Submit." These details will be added to the `config.ini` file.

4. Relaunch the app and click "Login." Now, it should be all set, and you should see "Login Success!" in the message area.

![image_2023-09-29_12-56-36](https://github.com/suresh-n/RichDotinScalperApp1/assets/17276643/6d3d0d1e-3117-434a-9031-2aa503e1088b)

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

**Left Arrow:** Initiates a Buy Call order.
**Right Arrow:** Initiates a Buy Put order.
**Key C:** Squares Off all or closes open positions.
**Key T:** Places a target order with predefined target points set in your settings.
**Key S:** Places a stop loss order with predefined stop loss points set in your settings.
**Key 1:** Initiates a trailing stop loss order with predefined trail stop points set in your settings.


### Feature Addition: Max Stop Loss
**Introducing Max MTM Stop Loss**

We're excited to present a new feature that allows you to set a maximum stop loss for enhanced risk management. Follow the simple instructions below to make the most of this feature:

![image](https://github.com/suresh-n/RichDotinScalperApp1/assets/17276643/869fa5c8-1e32-45c0-a9ab-4b4a747d4e97)


**Accessing Settings:**

Log in to your account and navigate to the 'Settings' section.
Enter your desired max MTM stop loss value and save the configuration.

**Activation:**

Below the login/logout button, locate the 'ON/OFF' toggle.
Switch it to 'ON,' and you'll notice it turning green, indicating that the feature is now active.

**Automated Square Off:**

Once the MTM breaches the negatively defined value, the tool will automatically execute the square-off logic to mitigate potential losses.

**Caution:**

Exercise caution while using this feature, as it may experience occasional failures due to network fluctuations or API issues.
Make your trading experience more secure and flexible with this powerful addition. Happy trading!


**We noticed the winows defender showing the our exe as virus please add file in exception on windows defender to make it work otherwise the app getting deleted.**
I'm working on the fix to this, as of now just turn off realtime protection in windows defender and add the exe to the exception then turn the realtime protection again.  

demo video : 📈 Free Index option Scalper App for Shoonya and Flattrade API - Demo 📉 #Shoonya#Flattrade #richdotin
https://youtu.be/kGtyJ5Ar64M
join telegram group by invite link: https://t.me/+RtOmEfaIn6JmMTg1

### Note
Please contact your financial adviser before placing your trade. We are not responsible for any trading loss or issues that occur due to broker API problems.
