## Theory

In general the Bureau of Reclamation [Water Measurement Manual (WMM)](https://www.usbr.gov/tsc/techreferences/mands/wmm/) is far and away the most commonly referenced guide. It is fairly complete but also quite prescriptive with limited formal references. One of the basic challenges of the weirs in the COID system is that the head height, h (water over the weir), is less than or near to 0.2 ft (2.4 in)  which is the limit of the applicable tables described in the previous page. Measurements of flow using Cipoletti weirs are already a little shaky ($\pm 5\%$). The flow depends exponentially on the h in the standard model and therefore small changes in the model might well complicate efforts to verify flow rates at different points in a ditch.

## Basic Model:

The basic model looks like this:

```{math}
:label: Sharp_Crested_Flow_Eqn

Q = \frac{2}{3}C_db\sqrt{2g}h^{\frac{3}{2}}
```

Where Q = volumetric flow rate,  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;b = width of the weir  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;g = gravitational constant  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Cd = discharge coefficient

In the (WMM) this is simplified to  

```{math}
:label: WMM Model

Q = 3.367bh^{\frac{3}{2}}
```
Where all measurements are in ft.

This appears to be based on the Rehbock model where 

```{math}
:label: Rehbock Model

C_{dR} = 0.611 + 0.075\frac{h}{P}
```
where P is the upstream depth to the crest. Applying this model to the: {eq}`Sharp_Crested_Flow_Eqn` yields the coefficient for {eq}`WMM Model` reasonably well.

To cite an item in the bibliography, use the citation key (from references.bib) with an @ prefix. For example, `@baker2016reproducibility` renders as @baker2016reproducibility.


[](https://doi.org/10.1061/JIDEDH.IRENG-10027) 

[](https://doi.org/10.1061/(ASCE)IR.1943-4774.0001652)

[Theory of Weirs: Class Notes- Sergio Maldonado](https://sergio-maldonado.github.io/teaching.html)

[](https://doi.org/10.1061/TACEAT.0004045)
