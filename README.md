I have a mining rig that based on the ASRock H110 Pro BTC that supports up to 13 GPUS (although my case only takes 12).

I have spent some time experimenting with windows and linux configurations trying to get the most stable and most efficient setup.

I note my findings down here in the hope that it might remind me what I did in the future and possibly help others out.

# Initial Hardware Build

I followed [this guide](http://www.cryptobadger.com/2017/04/build-ethereum-mining-rig-hardware/) on hardware selection. THe takeaways are cheap processor, not much memory, any hard drive.

Motherboard selection is important as this determines how many gpus you can use. More gpus per motherboard means less overhead power costs. I went for the  ASRock H110 Pro BTC as it supports 13. I also bought this [stackable frame](https://www.amazon.co.uk/dp/B0749F8TD9/ref=pe_3187911_189395841_TE_3p_dp_1) that supports 12 GPUs and 2 power supplies.

The hardware guide above recommends AMD RX 480 cards. I did buy a few of them but had issues overclocking them. They are also getting a bit old now and will have lower resale costs if you come to sell them later.

I went with Nvidia GTX 1070 cards that have a really fantasic power / output ratio when you overclock them.

# Linux Installation

[This guide](http://www.cryptobadger.com/2017/04/build-ethereum-mining-rig-linux/) gives you everything you need to know about installing linux and getting mining working.

# Overclocking

This is the tricky bit. Overclocking is easy on windows, you just install MSI after burner. It's not as easy on Linux.

With Nvidia cards you can use the `nvidia-settings` and `nvidia-smi` utilities that come with the driver to configure your cards but it is not very straight forward, particularly if you are using ssh rather than using the computer directly.

Eventually I found this REALLY helpful git repo: 

https://github.com/Cyclenerd/ethereum_nvidia_miner

This has an image to use directly that is setup to overclock and mine etherium with little or no additional configuration. I didn't use the image but I used the scripts to configure and overclock my cards.
