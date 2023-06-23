# SmallWhiteholeTestnetParser repo

# This is a simple Python script that reads raw csv data from arbiscan    #
# Made for Whitehole Testnet phase 2 to identify cheaters                 #
# v1.0                                                                    #
# # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # # #

# The list of gETH token transactions can be found here:
# https://goerli.arbiscan.io/token/0xd3e7076dd4513cf21bdee610cc5b144026631518
# Used because you get gETH for lending ETH
# Rules - you get more than 0.1 plus what you get from lending NFTs - you are a potential CHEATER
# How? Even if ETH has 0 farming potential, it still can be used to borrow USDT
# Borrowed USDT can buy you GRV tokens putting you ahead in competition due to external funding usage
# You can get 0.5 ETH by lending NFTs + 0.1 ETH was allowed to be supplied
# I would assume 0.6 ETH is the limit, 0.6-0.99 ETH is borderline questionable
# And from my point of view >1 ETH lent is clearly abusing external assets and breaking the rules

# !!! Please take note that this simple check can't determine if the address actually *USED* ETH to get GRV !!!
# !!! The only thing it can detect is lending more ETH than allowed !!!
