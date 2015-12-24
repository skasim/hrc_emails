## Network Analysis of Hillary Clinton's Emails

[Kaggle](https://www.kaggle.com), as part of a [competition](https://www.kaggle.com/c/hillary-clinton-emails), made available over 7,000 pages of emails sent by Hillary Clinton and her associates. I found the emails fascinating not just because of the content, but because they told a story about the inner workings of Clinton's inner circle. I used network analysis and matplotlib to visually demonstrate how Clinton's inner circle operated. You can view the code [here](https://github.com/skasim/hrc_emails/blob/master/hrc_network_analysis_with_graphs.ipynb).


## Hillary Clinton's Network

The graph below shows Clinton's network based on email senders and receivers who sent more than 10 emails to each other. Clinton, of course, is at the center of the network. However, there are also interesting patterns where secondary nodes (e.g., Huma Abedin and Lona Volmaro) are interacting with each other.

![alt tag](graphs/hrc_network.png)

It isn't surprising that Clinton is at the center of the network. Of the 7,000+ emails analyzed, Clinton is either a sender or a receiver in the top 15 sender-receiver pairs.

![alt tag](graphs/top15.png)

Another interesting aspect of this email story is what does the network look like when Clinton is not involved (i.e., how does information flow when Clinton is not a sender or receiver of the emails). In this case, we find that there is no one true central node. Instead, Abedin, Cheryl Mills, and Jake Sullivan are now the main arbiters of information.

![alt tag](graphs/other_network.png)

## To Run

Run in Jupyter using the below:

```
- Import Pandas
- Import sqlite3
- Import networkx
- Import matplotlib.pyplot
```