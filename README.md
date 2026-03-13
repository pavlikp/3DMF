# Volumetric Radar Echo Motion Estimation Using Physics-Informed Deep Learning: A Case Study Over Slovakia
This page contains interactive HTML figures from the paper Volumetric Radar Echo Motion Estimation Using Physics-Informed Deep Learning: A Case Study Over Slovakia.

## Abstract
Motion estimation from spatiotemporal Earth observation data is a key component of many forecasting and monitoring systems. In precipitation nowcasting, most extrapolation-based methods rely on two-dimensional radar composites to estimate the horizontal motion of precipitation systems. However, in some cases, precipitation systems can exhibit different motion directions at different heights. We propose a physics-informed convolutional neural network that estimates independent horizontal motion fields for multiple altitude layers directly from volumetric radar reflectivity data and investigate the practical benefits of altitude-wise motion field estimation for precipitation nowcasting. The model is trained end-to-end on volumetric observations from the Slovak radar network and its extrapolation nowcasting performance is evaluated. We compare the proposed model against an architecturally identical baseline operating on vertically pooled two-dimensional radar composites. Our results show that, although the model successfully learns altitude-wise motion fields, the estimated displacement is highly correlated across vertical levels for the vast majority of precipitation events. Consequently, the volumetric approach does not yield systematic improvements in nowcasting accuracy. While categorical metrics indicate increased precipitation detection at longer lead times, this gain is largely attributable to non-physical artifacts and is accompanied by a growing positive bias. A comprehensive inter-altitude motion field correlation analysis further confirms that events exhibiting meaningful vertical variability in horizontal motion are rare in the studied region. We conclude that, for the Slovak radar dataset, the additional complexity of three-dimensional motion field estimation is not justified by questionable gains in predictive skill. Nonetheless, the proposed framework remains applicable in climates where precipitation systems exhibit stronger vertical variability in horizontal motion.

Preprint link: XXX

## Figure 12
Vertically pooled CMAX representations of a severe precipitation event over Slovakia on July 5th 2022. The left image shows target radar observations and the right image the extrapolations obtained by advecting the final observation using the volumetric motion field estimated by the proposed 3D Motion Field U-Net. The estimated 3D motion field is vertically averaged and overlaid for reference. Zoomed regions highlight a non-physical cell-splitting artifact produced by the volumetric approach.

[Figure 12](fig12.html)

## Figure 16
Estimated horizontal motion fields and corresponding precipitation fields for three events selected for their low inter-altitude motion correlation and high precipitation coverage. The All Vertical Slices animations show a horizontal slice through the motion field for all altitudes, averlaid with a corresponding reflectivity measurement. The In Motion Animations show the estimated horizontal motion fields and corresponding precipitation fields at the lowest altitude layer (500–1000 m above ground level; left) and a mid-level layer (2500–3000 m above ground level; right).

### (a) 2022-04-09 09:55
[Figure 16 (a) All Vertical Slices](fig16_a_1.html)

[Figure 16 (a) In Motion](fig16_a_2.html)

### (b) 2021-05-17 05:50
[Figure 16 (b) All Vertical Slices](fig16_b_1.html)

[Figure 16 (b) In Motion](fig16_b_2.html)

### (c) 2019-11-05 20:30
[Figure 16 (c) All Vertical Slices](fig16_c_1.html)

[Figure 16 (c) In Motion](fig16_c_2.html)
