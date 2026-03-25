# Trend-surface-analysis
Trend surface analysis identifies systematic large-scale spatial variation (drift) in the given dataset.  A significant spatial trend indicates that the mean varies with location, violating the stationarity assumption of Ordinary Kriging. 

Steps to be followed:

1. Prepare rainfall data with longitude, latitude, and rainfall values of Andhra Pradesh and remove missing or erroneous records.

2. Import the data into MATLAB and extract coordinate and rainfall vectors.
  
3. Plot spatial distribution of rainfall to visually identify large-scale gradients (e.g., coastal to inland variation).
	
4. Select trend surface order (usually second-order polynomial for rainfall data).
   
5. Fit the trend surface model using polynomial regression (least squares method).

6. Generate the large-scale trend surface over the study area using a regular spatial grid.

7. Calculate residuals by subtracting trend values from observed rainfall.

8. Analyze residuals to ensure the large-scale trend is removed and only local variation remains.

9. Use trend information to select Kriging method, typically Universal Kriging for non-stationary rainfall data
