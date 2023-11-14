# DPRR and D-DPRR

**Authors:** Tian Lan, Tongfang Li

## Datasets

The "01-data" folder contains research data for Qinan, Weijiabao, Xianyang, Zhangjiashan, and Zhuangtou. Data types include:

### Meteorological data
   - air_pressure
   - wind_speed
   - temperature_avg
   - temperature_max
   - temperature_min
   - relative_humidity
   - precipitation
   - sunshine_duration
   - ET0 (calculated by the FAO Penman-Monteith equation)

### Other data
   - runoff
   - baseflow
   - NDVI
   - ISR
   - NTL
   - POP

## Main Analysis Codes

### DPRR

- `DPRR.py`: Calculation of DPRR based on DCCA and DPCCA. Results are stored in Excel format.
- `kde.py`: Calculation of the maximum kernel density corresponding value of the series.

### D-DPRR

- `D-DPRR.py`: Calculation of D-DPRR results under different step conditions. Results are stored in Excel format.

### Non-stationarity_ analysis

#### Trend Test

- `TFPW-MK.py`: The TFPW-MK method was used to test the trend.

#### Inconsistency Test

- `TFPW_Pettitt.m`: Storing the function used for inconsistency test.
- `TFPW_Pettitt_BS.m`: The TFPW-Pettitt-BS method was used to test inconsistency.

### Precipitation-runoff relationships

#### Violin for DCCA

- `Figure5a-violin-DCCA.py`: Drawing a violin plot based on DCCA results calculated by "DPRR.py".

#### Heatmap for DCCA

- `Figure5b-heatmap-DCCA.py`: Drawing a heatmap plot based on DCCA results calculated by "D-DPRR.py".

#### MIC for year

- `Figure5c-MIC_year.py`: Calculating the MIC results between pairs of ET0, BF, NDVI, ISR, NTL, and POP.

### Driving levels and directions

#### absolute value

- `Figure6a-violin-DPRR.py`: Drawing a violin plot based on DPRR results calculated by "DPRR.py".

#### Violin for absolute value of DPRR

- `Figure6b-violin-DPRR-abs.py`: Drawing a violin plot based on the absolute value of the DPRR results.

#### Heatmap for D-DPRR

- `Figure6c-heatmap-D-DPRR.py`: Drawing a heatmap plot based on D-DPRR results calculated by "D-DPRR.py".
