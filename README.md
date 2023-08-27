# Implementation-of-Propagation-Channels-and-Large-Small-scale-effects
In this repository, we delve into the examination of a telecommunications base station and the small-scale and large-scale effects on propagation channels, including shadowing and path loss. Finally, we investigate the Doppler shift effect on a specific channel.

The purpose of performing this exercise is to become familiar with the effects of the channel on received power. As we have become acquainted with these effects throughout the course, we can categorize them into two groups: large-scale effects and small-scale effects.

In the first part of the exercise, we delve into examining the large-scale effects. Two influential factors in these effects are path loss and shadowing. In this section, we consider a base station and plot graphs of the distribution of received power by users and the Signal-to-Noise Ratio (SNR) based on the distance of each user. Finally, we also investigate the probability of system outage in this communication system.

In the second part of the exercise, we study the small-scale effects. For this purpose, we consider a multi-path wireless channel and examine the channel impulse response from various angles in both wideband and narrowband scenarios.

**Part 1:** Analysis of Channel Effects on Received Signal Power

In this section, we consider a base station (BS) that serves $10^5$ mobile users distributed randomly within distances ranging from $d_0=10m$ to $D=1km=1000m$. The path loss is defined using the Simplified Path Loss Model with a path loss exponent of $n=4$. The average received power at a distance of $d_0=10m$ from the base station (BS) is $1μW$. Additionally, the white Gaussian noise power density at the receiver is $-175 dBm/Hz$. (We assume a signal bandwidth (B) of $1 MHz$.)

In reality, as the distance from the base station increases, the number of users within a specific radius should increase. In other words, the number of users within a 500m radius should be greater than within a 100m radius (this can be justified by calculating the area of two circles with different radii).

**1- Plotting the cumulative distribution function (CDF) of received power for each user**

![image](https://github.com/ErfanPanahi/Implementation-of-Propagation-Channels-and-Large-Small-scale-effects/assets/107314081/57eaac56-7641-4269-aa8c-99cd953d0f0d)


**2- SNR chart based on user distance**

![image](https://github.com/ErfanPanahi/Implementation-of-Propagation-Channels-and-Large-Small-scale-effects/assets/107314081/61b12c83-475a-45dd-9a61-3067f0da75b5)


**3- Considering the Shadow Effect**

![image](https://github.com/ErfanPanahi/Implementation-of-Propagation-Channels-and-Large-Small-scale-effects/assets/107314081/df7bf45f-6c6a-4256-89ac-d53ceb05774b)

![image](https://github.com/ErfanPanahi/Implementation-of-Propagation-Channels-and-Large-Small-scale-effects/assets/107314081/4d85f009-60fe-4697-96bd-19e1aa3b0fd7)


**4- Probability of outage versus user distance**

![image](https://github.com/ErfanPanahi/Implementation-of-Propagation-Channels-and-Large-Small-scale-effects/assets/107314081/cfe76ea8-8106-421b-ab90-1b6881f5e2d4)


**5- Probability of outage versus user distance**

![image](https://github.com/ErfanPanahi/Implementation-of-Propagation-Channels-and-Large-Small-scale-effects/assets/107314081/46f2aea9-923f-412a-aa13-f5c9a7a9cf09)

![image](https://github.com/ErfanPanahi/Implementation-of-Propagation-Channels-and-Large-Small-scale-effects/assets/107314081/6a281bd8-619a-4664-9cb8-109e0f4b53af)

**Part 2:** Multi-Path Wireless Channel Analysis

In this question, we intend to implement a multi-path wireless channel. For this purpose, we assume that 15 signals are received in clusters from 15 different paths with angles ranging from 0 to $π/2$ (uniformly distributed). Each path is modeled by a fading Rayleigh channel with a delay of $τ$ (uniform distribution from $1μs$ to $10μs$), and its average power is defined as $2σ^2 = 10^(-3) τ^(-4)$. (Here, $τ$ is in $μs$.)

Furthermore, in this channel, we consider a moving user with a velocity of $v = 30 m/s$. The carrier frequency is set as $f_c = 3 GHz$.

**1- Wide Band Channel**

![image](https://github.com/ErfanPanahi/Implementation-of-Propagation-Channels-and-Large-Small-scale-effects/assets/107314081/b22f68ed-fffe-4365-acf5-c009ac7e8b5b)


**2- Narrow Band Channel**

![image](https://github.com/ErfanPanahi/Implementation-of-Propagation-Channels-and-Large-Small-scale-effects/assets/107314081/588211d6-4095-491e-8b98-d004c0368d43)

![image](https://github.com/ErfanPanahi/Implementation-of-Propagation-Channels-and-Large-Small-scale-effects/assets/107314081/71514f68-89c8-4c60-8c01-2c62c5eda9de)
