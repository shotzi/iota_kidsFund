# iota_kidsFund
Pocket money management for kids 

# Motivation:

We have 3 kids 10, 12 and 16 years old. In the past there was a lot of confusion about how much money the kids already spend and if they got their pocket money already.  My wife tried to manage that in the past with putting notes into her mobile phone, but the kids did either manipulate the notes, discussed endlessly that they didn't get enough or that the notes where wrong. 

To make things even more complicate they transfered the money internally from one to another for different reasons. My wife than had to manage this transfer as well, which made things even worse.


# The Solution:

Set up an internal exchange/ trading plattform based on IOTA by using the trinity wallet. I tried it with the light wallet as well, but that was to difficult for the kids because of the missing currency exchange in the light wallet. 


# Advantage:

No more double spending to the kids. 

No more arguments and discussions about the current balance.

We are no longer needed for internal money transfer between the kids.

They have a documented list what they got and how much they spend and for what purpose. 

They learn about trading and exchanges. The oldest son (16) has already a binance acount. So he can try to increase his money by trading. If that doesn't work its his money he is loosing .

If the course goes up they benefit from the increase, but only if they didn't spend the money already.

They learn to not to spend the money and benefit from better exchange rates for iota in the long term.

They can't loose the money in case they loose their password, because you still have the seed.

They learn to set proper passwords for the wallet and that passwords are important. 


# Implementation: 

The central pocket money account is managed by my wife by using her mobile wallet. The account is filled with enough iotas for the next 3 month plus the start amount for each child for the initial setup.

I generated for each of them one seed and set up the wallet for them on there individual ipad. The only think they had to do was to set the password in the wallet. But even if they forget that, the iotas are not lost because I still have the seed.

To avoid the discussions with them about the possible losses, I increased the weekly pocketmoney by 30%. There where no complains . In the end that is far cheaper then the double and triple payouts we had in the past.

The initial start was done by manual transfer the money from the central wallet to their individual wallet. The next step will be the automatic transfer of the weekly pocketmoney (former +30%) on a daily base based on the daily exchange rate at 6 pm UTC. This is done by a python script and a cron job on running on a rasperry pi. So they get every day a small amount and the exchange rate does hopefully have not to much effect.

When they buy stuff for example in apple store, amazone, or they wan't EUR they have to transfer the amount in EUR to my wife (back into the pocketmoney account). This is easily done with the wallet (EUR transfer functionality and the barcode).


# Rollout:

We trained that yesterday and within 30 minutes the kids and my wife where able to transfer test iotas from one to another. This week we are testing it just with iotas. To make things easy for the tryout 1 EUR = 100 iota.

Next Monday we will switch to the process based on the exchange rate. Then every kid gets his initial amount based on EUR to the actual EUR rate.

The python script for the daily payout works so far, but the implementation based on the exchange rate is still missing, but there are many API where I can grep the value. So this wan't be a problem.


# Feel free to copy the idea and have fun. 

The next step is finalicing the phython script and put that in here as well.
