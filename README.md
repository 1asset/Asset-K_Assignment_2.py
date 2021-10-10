# Web Scrapping tool for Cryptocurrencies 
Asset Kanatov SE-2004

# Installing

#### Beautiful Soup 
`<pip install beautifulsoup4>`
#### Requests 
`<pip install requests>`

# Usage Examples
```
import requests
from bs4 import BeautifulSoup


class CryptoMarket:
    def data_retriever(self, crypto):
        url_link = 'https://coinmarketcap.com/currencies/' +crypto+ '/news/'
        request = requests.get(url_link, 'html.parser').text
        beautiful_soup = BeautifulSoup(request,'lxml')
        paragraph_heading = beautiful_soup.h1.text
        print(paragraph_heading)

        paragraph = beautiful_soup.text.strip()
        x = 0

        for i in range(len(paragraph)):
        
            print (paragraph[i], end ='')
            if paragraph[i] ==' ':
                x = x + 1
            if x == 5:
                print('\n', end='')
                x = 0
        print()
```

```
from assignment2 import CryptoMarket
output = CryptoMarket()
currency = input ('Input the cryptocurrency you want to output: ')
output.data_retriever (currency)
```

# Example with testing
#### You need to run the file test.py and then input the cryptocurrency in the terminal
#### For example input: Ethereum and you will get all related data for that coin
```
Ethereum Price (ETH)
Ethereum price today, ETH to 
USD live, marketcap and chart
| CoinMarketCapCryptos:  12,574Exchanges:  413Market Cap:
 $2,308,224,676,68524h Vol:  $92,153,301,032Dominance:  BTC: 45.1% ETH:
18.0%ETH Gas:  90 GweiCryptocurrenciesRankingRecently AddedPrice
EstimatesNewLegal Tender CountriesGlobal ChartsFiats /
Companies RankingSpotlightGainers & LosersHistorical SnapshotsExchangesSpotDerivativesDEXWhere
to BuyNFTOverall NFT StatisticsTop CollectionsPortfolioWatchlistCalendarsFree
AirdropsICO CalendarPolkadot ParachainsEvents CalendarProductsSwapsNewConverterMobile AppsBlockchain
ExplorerInterestJobs BoardCrypto APISite WidgetsLearnAlexandriaVideosNewEarnNewMarket UpdatesGlossaryNewsletterMethodologyCryptos:
 12,574Exchanges:  413Market Cap:  $2,308,224,676,68524h Vol:
 $92,153,301,032Dominance:  BTC: 45.1% ETH: 18.0%ETH Gas:
 90 GweiCryptocurrenciesCoinsEthereumEthereumETHRank #2CoinOn 1,882,342 watchlistsEthereum
Price (ETH)$3,521.651.89%0.0637 BTC2.74%Low:$3,492.57High:$3,603.2424h  Ethereum ETHPrice: $3,521.65 1.89%Add to
Main Watchlist  Market Cap$415,107,494,8121.88%Fully Diluted
Market Cap$415,107,494,8121.89%Volume 24h$14,691,947,05510.81%Volume / Market
Cap0.03539Circulating Supply117,872,849.44 ETHMax Supply--Total Supply117,872,849More
statsBuyExchangeGamingEarn CryptoSponsoredLinksWebsite, Explorers, Socials etc.WebsiteExplorersCommunityChatSource
codeWhitepaperEthereum LinksLinkswww.ethereum.orgen.wikipedia.org/wiki/Et...Source codeWhitepaperChatExplorersetherscan.ioethplorer.ioblockchair.combscscan.cometh.tokenview.comCommunitybitcointalk.orgforum.ethereum.orgethresear.chTwitterRedditContractsBinance Smart Chain
(BEP20)0x2170...9f933f8MoreBinance Smart Chain (BEP20)0x2170...9f933f8Ethereum ContractsBinance
Smart Chain (BEP20)0x2170...9f933f8TomoChain0x2eaa...cc7fb8bHeco0x64ff...428a1fdAvalanche C-Chain0xf20d...8fa6e15Sora0x0200...0000000Please change  
the wallet networkChange the wallet
network in the MetaMask Application
to add this contract.I understandTagsMineablePoW+28MineablePoWSmart
ContractsEthereumView allEthereum TagsConsensus AlgorithmPoWPropertySmart ContractsBinance
Smart ChainCoinbase Ventures PortfolioThree Arrows
Capital PortfolioPolychain Capital PortfolioBinance Labs
PortfolioArrington XRP capitalBlockchain Capital PortfolioBoostVC
PortfolioCMS Holdings PortfolioDCG PortfolioDragonFly Capital
PortfolioElectric Capital PortfolioFabric Ventures PortfolioFramework
VenturesHashkey Capital PortfolioKinetic CapitalHuobi CapitalAlameda
Research PortfolioA16Z Portfolio1Confirmation PortfolioWinklevoss CapitalUSV
PortfolioPlaceholder Ventures PortfolioPantera Capital PortfolioMulticoin
Capital PortfolioParadigm XZY ScreenerPlatformEthereumOtherMineableOverviewMarketHistorical DataProject
InfoWalletsNewsSocialsRatingsAnalysisPrice EstimatesShareEthereum to USD ChartLoading
DataPlease wait, we are loading
chart dataETH Price Live DataThe
live Ethereum price today is
$3,521.65 USD with a 24-hour
trading volume of $14,691,947,055 USD.
We update our ETH to
USD price in real-time. Ethereum
is down 1.89% in the
last 24 hours. The current
CoinMarketCap ranking is #2, with
a live market cap of
$415,107,494,812 USD. It has a
circulating supply of 117,872,849 ETH
coins and the max. supply
is not available.If you would
like to know where to
buy Ethereum, the top exchanges
for trading in Ethereum are
currently Binance, Huobi Global, Mandala
Exchange, OKEx,  and FTX.
You can find others listed
on our crypto exchanges page.What
Is Ethereum (ETH)?Ethereum is a
decentralized open-source blockchain system that
features its own cryptocurrency, Ether.
ETH works as a platform
for numerous other cryptocurrencies, as
well as for the execution
of decentralized smart contracts.Ethereum was
first described in a 2013
whitepaper by Vitalik Buterin. Buterin,
along with other co-founders, secured
funding for the project in
an online public crowd sale 
in the summer of 2014.
The project team managed to
raise $18.3 million in Bitcoin,
and Ethereum’s price in the
Initial Coin Offering (ICO) was
$0.311, with over 60 million
Ether sold. Taking Ethereum’s price
now, this puts the return
on investment (ROI) at an
annualized rate of over 270%,
essentially almost quadrupling your investment
every year since the summer
of 2014.The Ethereum Foundation officially
launched the blockchain on July
30, 2015, under the prototype
codenamed “Frontier.” Since then, there
has been several network updates
— “Constantinople” on Feb. 28,
2019, “Istanbul” on Dec. 8,
2019, “Muir Glacier” on Jan.
2, 2020, “Berlin” on April
14, 2021, and most recently
on Aug. 5, 2021, the
“London” hard fork.Ethereum’s own purported
goal is to become a
global platform for decentralized applications,
allowing users from all over
the world to write and
run software that is resistant
to censorship, downtime and fraud.Who
Are the Founders of Ethereum?Ethereum
has a total of eight
co-founders — an unusually large
number for a crypto project.
They first met on June
7, 2014, in Zug, Switzerland.Russian-Canadian
Vitalik Buterin is perhaps the
best known of the bunch.
He authored the original white
paper that first described Ethereum
in 2013 and still works
on improving the platform to
this day. Prior to ETH,
Buterin co-founded and wrote for
the Bitcoin Magazine news website.British
programmer Gavin Wood is arguably
the second most important co-founder
of ETH, as he coded 
the first technical implementation of
Ethereum in the C++ programming
language, proposed Ethereum’s native programming
language Solidity and was the
first chief technology officer of
the Ethereum Foundation. Before Ethereum,
Wood was a research scientist
at Microsoft. Afterward, he moved
on to establish the Web3
Foundation.Among the other co-founders of
Ethereum are: - Anthony Di
Iorio, who underwrote the project
during its early stage of
development. - Charles Hoskinson, who
played the principal role in
establishing the Swiss-based Ethereum Foundation
and its legal framework. -
Mihai Alisie, who provided assistance
in establishing the Ethereum Foundation.
- Joseph Lubin, a Canadian
entrepreneur, who, like Di Iorio,
has helped fund Ethereum during
its early days, and later
founded an incubator for startups
based on ETH called ConsenSys.
- Amir Chetrit, who helped
co-found Ethereum but stepped away
from it early into the
development.What Makes Ethereum Unique?Ethereum has
pioneered the concept of a
blockchain smart contract platform. Smart
contracts are computer programs that
automatically execute the actions necessary
to fulfill an agreement between
several parties on the internet.
They were designed to reduce
the need for trusted intermediates
between contractors, thus reducing transaction
costs while also increasing transaction
reliability.Ethereum’s principal innovation was designing
a platform that allowed it
to execute smart contracts using
the blockchain, which further reinforces
the already existing benefits of
smart contract technology. Ethereum’s blockchain
was designed, according to co-founder
Gavin Wood, as a sort
of “one computer for the
entire planet,” theoretically able to
make any program more robust,
censorship-resistant and less prone to
fraud by running it on
a globally distributed network of
public nodes.In addition to smart
contracts, Ethereum’s blockchain is able
to host other cryptocurrencies, called
“tokens,” through the use of
its ERC-20 compatibility standard. In
fact, this has been the
most common use for the
ETH platform so far: to
date, more than 280,000 ERC-20-compliant
tokens have been launched. Over
40 of these make the
top-100 cryptocurrencies by market capitalization,
for example, USDT, LINK and
BNB. Since the emergence of
Play2Earn games, there has been
a substantial increase in interest
in the ETH to PHP
price.Ethereum London Hard ForkThe Ethereum
network has been plagued with
high transaction fees, often buckling
at seasons of high demand.
In May 2021, the average
transaction fee of the network
peaked at $71.72.In addition to
the high cost of transactions,
the leading altcoin also suffers
from scalability issues.As already mentioned,
there are plans to transition
to a proof-of-stake algorithm in
order to boost the platform’s
scalability and add a number
of new features. The development
team has already begun the
transition process to ETH 2.0,
implementing some upgrades along the
way, including the London hard
fork.The London upgrade went live
in August 2021. It included
five Ethereum Improvement Proposals (EIPs),
namely EIP-3529, EIP-3198, EIP-3541, and
most notably EIP-1559 and EIP-3554.EIP-1559
is arguably the most popular
upgrade out of all the
EIPs.What Is EIP-1559?The EIP-1559 upgrade
introduces a mechanism that changes
the way gas fees are
estimated on the Ethereum blockchain. 
Before the upgrade, users had
to participate in an open
auction for their transactions to
be picked up by a
miner. This process is known
as a “first-price auction,” and
as expected, the highest bidder
wins. With EIP-1559, this process
is handled by an automated
bidding system, and there is
a set “base fee” for
transactions to be included in
the next block. This fee
varies based on how congested
the network is. Furthermore, users
who wish to speed up
their transactions can pay a
“priority fee” to a miner
for faster inclusion.EIP-1559 also introduces
a fee-burning mechanism. A part
of every transaction fee (the
base fee) is burned and
removed out of circulation. This
is intended to lower the
circulating supply of Ether and
potentially increase the value of
the token over time.Interestingly, less
than two months after the
London upgrade was implemented, the
network had burned over $1
billion worth of Ether.Related Pages:New
to crypto? Learn how to
buy Bitcoin today.Want to keep
track of Ethereum price live?
Download the CoinMarketCap mobile app!Want
to look up a transaction?
Visit our block explorer.Curious about
the crypto space? Read our
educational section — Alexandria.How Many
Ethereum (ETH) Coins Are There
In Circulation?In September 2021, there
were around 117.5 million ETH
coins in circulation, 72 million
of which were issued in
the genesis block — the
first ever block on the
Ethereum blockchain. Of these 72
million, 60 million were allocated
to the initial contributors to
the 2014 crowd sale that
funded the project, and 12
million were given to the
development fund.The remaining amount has
been issued in the form
of block rewards to the
miners on the Ethereum network.
The original reward in 2015
was 5 ETH per block,
which later went down to
3 ETH in late 2017
and then to 2 ETH
in early 2019. The average
time it takes to mine
an Ethereum block is around
13-15 seconds.In the August 2021
Ethereum network upgrade, the London
hard fork contained the Ethereum
Improvement Protocol, EIP-1559. Instead of
the first-price auction mechanism where
the highest bidder wins, EIP-1559
introduces a “base fee” for
transactions to be included in
the next block. Users that
want to have their transaction
prioritized can pay a “tip”
or “priority fee” to miners.
As the base fee adjusts
dynamically with transaction activity, this
reduces the volatility of Ethereum
gas fees, although it does
not reduce the price, which
is notoriously high during peak
congestion on the network.One of
the major differences between Bitcoin
and Ethereum’s economics is that
the latter is not deflationary,
i.e. its total supply is
not limited. Ethereum’s developers justify
this by not wanting to
have a “fixed security budget”
for the network. Being able
to adjust ETH’s issuance rate
via consensus allows the network
to maintain the minimum issuance
needed for adequate security.With the
introduction of EIP-1559 however, the
base fees used in transactions
are burned, removing the ETH
from circulation. This means higher
activity on the network would 
lead to more ETH burned,
and the decreasing supply should
lead to appreciation of Ethereum
price, all things equal. This
has the potential to make
Ethereum deflationary, something ETH holders
are excited about — a
potential appreciation in Ethereum price
today.How Is the Ethereum Network
Secured?As of August 2020, Ethereum
is secured via the Ethash
proof-of-work algorithm, belonging to the
Keccak family of hash functions.There
are plans, however, to transition
the network to a proof-of-stake
algorithm tied to the major
Ethereum 2.0 update, which launched
in late 2020.After the Ethereum
2.0 Beacon Chain (Phase 0)
went live in the beginning
of December 2020, it became
possible to begin staking on
the Ethereum 2.0 network. An
Ethereum stake is when you
deposit ETH (32 ETH is
required to activate validator software)
on Ethereum 2.0 by sending
it to a deposit contract,
thus helping to secure the
network by storing data, processing
transactions and adding new blocks
to the blockchain. At the
time of writing in mid-September
2021, the Ethereum price now
for 32 Ether is roughly
$116,029. The amount of money
earned by Ethereum validators right
now is a return of
6% APR, which equates to
around 1.91952 ETH, or $6960
in Ethereum price today. This
number will change as the
network develops and the amount
of stakers (validators) increase.Ethereum staking
rewards are determined by a
distribution curve (the participation and
average percent of stakers): some
ETH 2.0 staking rewards were
at 20% for early stakers,
but will be lowered to
end up between 7% and
4.5% annually. The minimum requirements
for an Ethereum stake are
32 ETH. If you decide
to stake in Ethereum 2.0,
it means that your Ethererum
stake will be locked up
on the network for months,
if not years, in the
future until the Ethereum 2.0
upgrade is completed.Where Can You
Buy Ethereum (ETH)?Given the fact
that Ethereum is the second-largest
cryptocurrency after Bitcoin, it is
possible to buy Ethereum, or
use ETH trading pairs on
nearly all of the major
crypto exchanges. Some of the
largest markets include:BinanceCoinbase ProOKExKrakenHuobi GlobalTo
check Ethereum price live in
the fiat currency of your
choice, you can use CoinMarketCap’s
converter feature directly on the
Ethereum currency page. Alternatively, use
the dedicated exchange rate converter
page. Popular Ethereum price pairs
include: ETH/USD, ETH/GBP, ETH/AUD and
ETH/JPY.Our most recent articles about
Ethereum:Ethereum Developer Pleads Guilty to
Violating North Korean SanctionsNFT of
Side Eyeing Chloe, Legendary Internet
Meme, Sells for 25 ETHNetflix
Making Show about 'Suspicious' Death
of Crypto Exchange BossCoinMarketCap Daily,
Sept. 27: BTC and ETH
Shrug Off China WoesCoinMarketRecap Podcast:
Crypto Drama, Snoop Dogg Bombshell,
NFTs for Afghanistan, CBDCs ExplainedRead
MoreETH to USD ConverterETHEthereumUSDUnited States
DollarETH Price StatisticsEthereum Price TodayEthereum
Price$3,521.65Price Change24h$-67.871.89%24h Low / 24h
High$3,492.57 /$3,603.24Trading Volume24h$14,691,947,055.3610.81%Volume / Market
Cap0.03539Market Dominance18.02%Market Rank#2Ethereum Market CapMarket
Cap$415,107,494,812.071.88%Fully Diluted Market Cap$415,107,494,812.071.89%Ethereum Price
YesterdayYesterday's Low / High$3,544.64 /$3,628.24Yesterday's
Open / Close$3,560.00 /$3,575.72Yesterday's Change0.44%Yesterday's
Volume$12,707,036,941.64Ethereum Price History7d Low /
7d High$3,283.45 /$3,667.9630d Low /
30d High$2,676.41 /$3,673.3190d Low /
90d High$1,722.05 /$4,022.4752 Week Low
/ 52 Week High$362.60 /$4,362.35All
Time HighMay 12, 2021 (5
months ago)$4,362.3519.27%All Time LowOct 21,
2015 (6 years ago)$0.4209836602.28%Ethereum ROI124268.91%Ethereum 
SupplyCirculating Supply117,872,849 ETHTotal Supply117,872,849 ETHMax
SupplyNo DataShow moreTrending Coins and
Tokens 🔥Hold BNB on BinanceAnd
Get 25% Off Trading Fees.Trade
NowSponsoredArivaARV#659FOMO BABYFOMOBABY#3017Beyond ProtocolBP#246Empire TokenEMPIRE#2897Frosted CakeFROSTEDCAKE#3002
People Also WatchElrond$246.91 -2.36%Uniswap$24.99 -5.33%UNION
Protocol Governance Token$0.01305 -8.75%Wise Token$0.5406
1.96%USD Coin$0.9994 -0.05%TrustSwap$0.9448 -7.61%Swap ETHProductsBlockchain
ExplorerCrypto APICrypto IndicesInterestJobs BoardSitemapCompanyAbout usTerms
of usePrivacy PolicyDisclaimerMethodologyCareersWe’re hiring!SupportRequest FormContact
SupportFAQGlossarySocialsFacebookTwitterTelegramInstagramInteractive Chat© 2021 CoinMarketCap. All
rights reserved
```

### If you got similar output, your code works fine
