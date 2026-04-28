---
title: Weir Theory

---

## Theory

In general the Water Measurement Manual @WMM2001USBR is far and away the most commonly referenced guide. It is fairly complete but also quite prescriptive with limited formal references. One of the basic challenges of the weirs in the COID system is that the head height, h (water over the weir), is less than or near to 0.2 ft (2.4 in)  which is the limit of the applicable tables described in the previous page. Measurements of flow using Cipoletti weirs are already a little shaky ($\pm 5\%$). The flow depends exponentially on the h in the standard model and therefore small changes in the model might well complicate efforts to verify flow rates at different points in a ditch.

## Basic Model:

The basic model looks like this (described in Sergio Maldonado's class notes: @maldonado2004theory) :

```{math}
:label: Sharp_Crested_Flow_Eqn

Q = \frac{2}{3}C_db\sqrt{2g}h^{\frac{3}{2}}
```

Where Q = volumetric flow rate,  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;b = width of the weir  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;g = gravitational constant  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Cd = discharge coefficient

In the @WMM2001USBR this is simplified to  

```{math}
:label: WMM Model

Q = 3.367bh^{\frac{3}{2}}
```
Where all measurements are in ft.

This appears to be based on the Rehbock model (described inwhere 

```{math}
:label: Rehbock Model

C_{dR} = 0.611 + 0.075\frac{h}{P}
```
where P is the upstream depth to the crest. Applying this model to the: {eq}`Sharp_Crested_Flow_Eqn` yields the coefficient for {eq}`WMM Model` reasonably well.

A great deal of this work goes back to empirical work originally done by @schroder1929weirprecise and others and commented on by @king1929weirdiscussion in 1929. The image below shows some of the original data for a Cipoletti weir and affirms the basic features of the Rehbock model. In this plot the head is measured in ft!

```{figure} ../Images/KingSchroderEmpirical1
:label: Schroder Empirical Data 1
:alt: Schroder Empirical Data 1
:width: 500 px
:align: center

Data from @king1929weirdiscussion
```

The following data from the same paper looks at the discharge coefficient as a function of head for a couple of different weir heights (P in modern language). This is not an exact comparison since these appear to have been uncontracted weirs (no restrictions on the ends). Never the less this provides some level of confirmation that the basic weir flow formulas have merit. Note that in this plot the discharge coefficient C$_d$ is the same as $\mu_0$. **Note:** In this plot the head is measured in m!

```{figure} ../Images/KingSchroderEmpirical2
:label: Schroder Empirical Data 2
:alt: Schroder Empirical Data 2
:width: 500 px
:align: center

Data from @king1929weirdiscussion
```

The feature of both plots that I think is relevant is that for heads in the range of $0.2 < h < 1.0$ the coefficient varies by less that 10%. A relevant feature of both plots is that the discharge coefficient increases as the head drops below 0.2 ft or 0.08 m.

This is consistent with the work in the paper @sinclair2022insights as well as commentary by @yao2023discuss.

```{figure} ../Images/SinclairData.png
:label: Sinclair Flow Model
:alt: Sinclair Flow Model
:width: 500 px
:align: center

Data from @sinclair2022insights
```
...and....

```{figure} ../Images/YaoData.png
:label: Yao Commentary
:alt: Yao Commentary
:width: 500 px
:align: center

Data from @yao2023discuss
```

### Conclusions

My current interpretation from this data is that {eq}`WMM Model` is a reasonable starting point. It feels important to remember that most of the weirs laterals and private laterals in the COID system seem to be operating below h = 0.2. Based on the data the actual flows are likely to be greater than the simple calculation would imply due to some increase in the discharge coefficient. How much greater is pretty clearly an open question at this time.
