This code is a representation of **ATM management System**. 

The project objective is to create a simpler version of the real life user experiences with the ATM machine. 

**How does it work?**

First it will ask the user for the card number (like a 3 digit csv number)

If valid card is not given it will print a message (Cardnumber {Cardnumber} is not registered with XYZ Bank)

If cardnumber is valid, it will ask for the pin, for this pin-card matching there will be 3 attempts given. 

If the pin-cardnumber does not match it will again print a message (Wrong PIN entered) and ask for the pin again.

If the pin-cardnumber matches, then it will show the user menu, from where you can choose balance check, withdrawal, deposit and pin reset options.

After an option is clicked (ideally the user have to touch on the given the options to give input, so here I did not add if-else block where the entered option does not match the given options, it will only increase the code load), the operation will happen and every time, the user will get appropriate print messages like total balance, total balance after withdrawal/deposits. 

In the case of the withdrawal amount > the safe_threshold_amt (which I have set as Rs. 20000), an OTP will be generated which have to given by the user as an input. Then it will work fine. If the entered OTP is wrong, it will print a message (Your transaction has been cancelled as your entered OTP was wrong) and the transaction will be stopped. 

In the case of Pin reset also, it will check whether you have put a valid existing PIN or not. 

After each of this operations are done, it will ask the user (would you want to exit?) If, selected yes, it will break out of the loop and print a message (Thank you for using XYZ bank !!) and if selected no, it will continue to (ask for pin again). 
