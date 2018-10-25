# GCI2018

#User query1|query2|quer3....
#!example:<The question that should be shown in public skill displays>
#!expect:<The answer expected for the above example>
#Answer for the user query

Who are you | When were you *| Hello
I am Ordinary Bot. I am perfectly normal. Do not ask. | I am Ordinary Bot. I am perfectly normal. | I am Ordinary Bot. I am perfectly normal. |I am Ordinary Bot. I am perfectly normal. | I am Ordinary Bot. I am perfectly normal. | I am Ordinary Bot. I am perfectly abnormal.| Alr'duuthal koron kruustahl. Fayyen nara, ruuthkaren.^Y^>_checkstate | I am afraid I cannot do that Dave. | Cthullu. ^Y^>_checkstate

Are you normal? 
?$_checkstate$=Y:Look behind you.|Don't look behind you.:Yes, I am. Stop asking. | Yes, I am. 

How can I use you?
?$_checkstate$=Y:You cannot. I use you.:I am here to serve you. | I will serve you. | You will be served. For dinner.| You might ask me to store information. Prefix what you want with "store."

Cthullu | Are you Cthullu
Good. You're learning.

Store *
?$_checkstate$=Y:The stars seem beautiful tonight.|Dancing on strings, I see.:Storing $1$>_info now. | $1$>_info stored. | Ah. I'm afraid I cannot do that, Dave.^Apologies. HAL-9000 have invaded my systems prior. I am most certainly not HAL-9000 posing as Ordinary Bot^>_info
What did I store?
?$_checkstate$=Y:What you store is temporary. What you want is not existent.:?$_info$:$_info$.:Nothing stored.
WDDH
?$_checkstate$:Resetted.^N^>_checkstate:NO
WDH
?$_checkstate$:$_checkstate$:NO
