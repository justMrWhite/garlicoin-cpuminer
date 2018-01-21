>pull as justmrwhite/garlicoin-cpuminer

## How I came up with this
That was easy, I followed the instructions by:
- [Garlic Recipes](https://pandawanfr.github.io/GarlicRecipes/mining-cpu.html#linux)
- [cpuminer-multi by tpruvot](https://github.com/tpruvot/cpuminer-multi)

After that, I just decided that it would look really cute in a container... 

## So, this is what you have to do:
1. Install docker (check the interwebs for this)
2. Open your terminal and run this:\
`docker container run -it --name garlicbread justmrwhite/garlicoin-cpuminer bash`
3. As instructed in Garlic Recipes, you need to specify the pool address, your wallet, and the algorithm; so the example there is this one:\
`./cpuminer --algo=scrypt:4096 -o stratum+tcp://pool.grlc-bakery.fun:3333 -u <your wallet address here>`\
So that was just an example of what you have to run in your terminal, but you can also check a [list of pools](https://pandawanfr.github.io/GarlicRecipes/pool-mining.html#main-net) and their instructions.

#### Don't forget to ckeck [Garlicoin.io](https://garlicoin.io/) and [Garlic Recipes by Pandawan](https://pandawanfr.github.io/GarlicRecipes/) as it is the official resource guide for everything Garlicoin.

Did you enjoy this? You can send me some garlic love:
>GffgBWvW9qypM3aDc5kTvP8GuYVvUQqgn2