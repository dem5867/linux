Mainline linux kernel for Orange Pi PC/One
------------------------------------------

This kernel tree is meant for Onrage Pi PC and Orange Pi One. 

(You can easily port it to other similar H3 based SBCs by modifying the
appropriate board DTS files. Usually these boards are either like Orange Pi One,
or like Orange Pi PC, or they don't have CPUX voltage regulation at all, so it
should be simple.)

Features in addition to mainline:

- CPU frequency and voltage scaling (cpufreq)
- Thermal regulation (if CPU heats above certain temperature, it will try to cool itself down by reducing CPU freqency)
- Ethernet driver v5 from [montjoie](https://github.com/montjoie/linux/commits/sun8i-emac-wip-v5)
- Working HDMI driver (v6 patches from [moinejf](http://moinejf.free.fr/opi2/) ported to sunxi-ng clk driver)
- USB OTG port works (you can create USB gadgets using Orange Pi)

Missing:

- Audio support
- Video decoding support

Have fun!
