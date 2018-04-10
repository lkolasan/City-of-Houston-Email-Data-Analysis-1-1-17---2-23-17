Data includes: Sender To CC BCC Sent date/time Received date/time Assembled by Matt Chapman (hubblefisher@gmail.com) through FOIA request.

I use the dataset to determine a. communities / teams b. machine generated emails c. well-connected / trustworthy-people in this dataset

Thought process:

Identifying Machine generated emails: Heavy receiver and sender must be just a busy person but the combination of heavy sender and low receiver should be machine. Machines would show imbalance between sending and receiving behavior. Also Machines won't send to other machines most likely which may help out the categorization further.

Well-connected / Trustworthy people: Well-connected / trustworthy-people are those who have history of "receiving" any emails plus those who have multiple email exchange history with certain emails seemingly communicating with others instead of one-time, one-way communication.

Finding the Communities/ Teams in the dataset: To distinguish communities/teams, I used Frequent pattern mining. First I filter out all the machine generated emails from above analysis. Similar to Market basket analysis, I would take each email as a transaction and the email ids present in it as products. Then, I took a subset of data having bulk email ids. Using FP growth algorithm, We could identify the most coomunicating groups of people by applying threshold for size of teh group.(One more normal approach is to use clustering by creating a space matrix of email ids. Compare both the results and pick the one which gives the best results. Checking for strings that appear most in Receiver, CC, BCC might also give an idea of the groups.)
