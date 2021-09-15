# Locate River Junction

In this project I have to Locate the river Junction from a Satelite (.tif) Image. In addition to that I have to Find the Flow Accmulation, Flow Diretion etc.

## Slope
```
slope = rd.TerrainAttribute(shasta_dem, attrib='slope_riserun')
rd.rdShow(slope, axes=False, cmap='magma', figsize=(8, 5.5))
plt.show()
```

![slope](https://user-images.githubusercontent.com/39759685/133444593-20e00460-978c-4677-8962-42edf0f8350e.png)


## Aspect
```
aspect = rd.TerrainAttribute(shasta_dem, attrib='aspect')
rd.rdShow(aspect, axes=False, cmap='jet', figsize=(8, 5.5))
plt.show()
```

![Aspect](https://user-images.githubusercontent.com/39759685/133444713-a059a853-40eb-4223-bf05-3b8dc34cfa86.png)

## Flow Accmulation

```
accum = rd.FlowAccumulation(shasta_dem , method='Rho8' , in_place=True)
d8_fig = rd.rdShow(accum, zxmin=350, zxmax=750, zymin=1550, zymax=1050, figsize=(8,5.5), axes=False , cmap ='jet')
```

![Flow Accmulation](https://user-images.githubusercontent.com/39759685/133444830-76b0f92c-3ffa-4749-acb3-bc523d75fbf8.png)


## Grayscale image
In the following Images There are lots of noise, That Problem i have to tackel next

![grayscale](https://user-images.githubusercontent.com/39759685/133445438-693d2603-48ba-4f1e-97be-72480ec63132.png)


## Skinned Image
I have extraced the Network of the river using the `sklearn` library

![skinned](https://user-images.githubusercontent.com/39759685/133445789-ff472191-a069-4215-8d48-19f0c355ba9f.png)

## Denoised Image

![remove_obj](https://user-images.githubusercontent.com/39759685/133445936-daf0c72f-5382-41c6-9f8c-094670ce2c17.png)

## Junctions FINALLY!!

I have used Several Morpholy to get those Points, For details see the Code

![final_black](https://user-images.githubusercontent.com/39759685/133446195-c21af174-d10f-4fd2-8eda-a08ef3655739.png)



