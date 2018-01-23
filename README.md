>pull as justmrwhite/garlicoin-cpuminer

## How I came up with this
That was easy, I followed the instructions by:
- [Garlic Recipes](https://pandawanfr.github.io/GarlicRecipes/mining-cpu.html#linux)
- [cpuminer-multi by tpruvot](https://github.com/tpruvot/cpuminer-multi)

After that, I just decided that it would look really cute in a container... 

## Start the fun:
1. Install docker (check the interwebs for this)
2. Open your terminal and run this:\
`docker container run -it --name garlicbread justmrwhite/garlicoin-cpuminer bash`\
you can replace *garlicbread* for whatever name you want to give your container (I would suggest the name of the pool).
3. As instructed in Garlic Recipes, you need to specify the pool address, your wallet, and the algorithm; so the example is this one to also run in your terminal:\
`./cpuminer --algo=scrypt:4096 -o stratum+tcp://pool.grlc-bakery.fun:3333 -u <your wallet address here>`\
That was just an example, but you can also check a [list of pools](https://pandawanfr.github.io/GarlicRecipes/pool-mining.html#main-net) and their instructions.

## To exit and remove the container:
In your terminal:
1. `ctrl c`
2. `exit`
3. `docker container rm garlicbread`\
to remove the container (which I suggest so it won't run more layers on top) or:

## To restart the container
I don't suggest restarting, just removing (above)
1. `docker container start -ai garlicbread`
2. Follow step 3 from *Start the fun*

#### Don't forget to ckeck [Garlicoin.io](https://garlicoin.io/) and [Garlic Recipes by Pandawan](https://pandawanfr.github.io/GarlicRecipes/) as it is the official resource guide for everything Garlicoin.

Did you enjoy this? You can send me some garlic love:
>Gfkokuadnhq27GZMUuVzf1SehYWWkesK4q