# Tinkering-with-a-TVAR-Model

__1.	Problem Statement__

The task involves working with a non-stationary signal, such as the El Centro ground motion data, or alternatively, creating a simulated non-stationary signal with similar characteristics. The objective is to apply a 3rd-order Time-Varying Autoregressive (TVAR) model to the signal and analyze its behavior. This will involve estimating the AR coefficients over time using a sliding window approach. Once the coefficients are obtained, it is required to create a coefficient cluster map, also known as a heatmap, to visualize how these coefficients evolve over time. The heatmap should have time or time windows on the X-axis, AR coefficient indices (1st, 2nd, and 3rd) on the Y-axis, and the color gradient should represent the magnitude of the coefficients.
In addition to generating the heatmap, an analysis explaining how the changes in the AR coefficients reflect the signal's non-stationary behavior should be provided. The analysis should include a discussion of any trends, patterns, or anomalies observed in the coefficient cluster map. The deliverables for this task include a clear and well-labeled heatmap and a short report explaining the methodology, results, and interpretation.

__2.	Abstract__

For this task, I have first generated a Non-stationary Time Series. Since Time-varying Autoregression (TVAR) Models can operate on a non-stationary time series, I have not converted the time series to stationary. Since the statsmodels library does not directly support time-varying parameters, I have created a custom implementation. I have then generated a heatmap of the autoregression (AR) coefficients, and drawn conclusions regarding the non-stationary nature of the data from it.
