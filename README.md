# Ebay-Auction-House
As you probably know, there is a multitude of online auction systems on the web. The most popular
one is eBay. I suggest that you visit this web site (although I suppose all of you have visited it
many times) to get an understanding of the look-and-feel of an auction web site and how such a
system is supposed to function.
The basic idea behind your online auction system is that it is intended to support a company that
lets users buy and sell an item in an on-line auction. (Think eBay. So we will call the company that
hired you BuyMe. If you are not familiar with how eBay works, please go to eBay to look for
something to buy, and look at eBay's FAQ/Help pages. )
In general, a seller posts an item for sale, starting an auction, which will close at a specified date
and time. The seller also posts an initial price, an increment for bids [which indicates a lower
bound on how much must be added to current bid for the next valid bid] and a (secret) minimum
price [the seller is not willing to give up the item for less]. Potential buyers post bids as part of the
auction, and the user with the highest bid at closing time gets to buy the item. (Actually, they must
buy the item.) The process of bidding is described in the above Help pages. The one fancy thing
you need to implement is "automatic bidding", which involves the buyer setting a (secret) upper
limit on how much they are willing to pay; every time someone bids higher than your current bid,
the computer automatically puts in a higher bid for you, till your upper limit is reached. So if there
is not much bidding, you may get the item for less than your upper limit. If someone bids past your
upper limit, BuyMe will alert you.
