# DPRR and D-DPRR

**Authors:** Tian Lan, Tongfang Li

## Datasets

The "01-data" folder contains research data for Qinan, Weijiabao, Xianyang, Zhangjiashan, and Zhuangtou. Data types include:

1. Meteorological data:
   - air_pressure
   - wind_speed
   - temperature_avg
   - temperature_max
   - temperature_min
   - relative_humidity
   - precipitation
   - sunshine_duration
   - ET0 (calculated by the FAO Penman-Monteith equation)

2. Other data:
   - runoff
   - baseflow
   - NDVI
   - ISR
   - NTL
   - POP

## Main Analysis Codes

### 02-DCCA+DPRR

- `DPRR.py`: Calculation of DPRR based on DCCA and DPCCA. Results are stored in Excel format.
- `kde.py`: Calculation of the maximum kernel density corresponding value of the series.

### 03-DCCA+D-DPRR

- `D-DPRR.py`: Calculation of D-DPRR results under different step conditions. Results are stored in Excel format.

### 04-Figure4

#### Trend Test

- `TFPW-MK.py`: The TFPW-MK method was used to test the trend.

#### Inconsistency Test

- `TFPW_Pettitt.m`: Storing the function used for inconsistency test.
- `TFPW_Pettitt_BS.m`: The TFPW-Pettitt-BS method was used to test inconsistency.

### 05-Figure5

#### Figure5a

- `Figure5a-violin-DCCA.py`: Drawing a violin plot based on DCCA results calculated by "DPRR.py".

#### Figure5b

- `Figure5b-heatmap-DCCA.py`: Drawing a heatmap plot based on DCCA results calculated by "D-DPRR.py".

#### Figure5c

- `Figure5c-MIC_year.py`: Calculating the MIC results between pairs of ET0, BF, NDVI, ISR, NTL, and POP.

### 06-Figure6

#### Figure6a

- `Figure6a-violin-DPRR.py`: Drawing a violin plot based on DPRR results calculated by "DPRR.py".

#### Figure6b

- `Figure6b-violin-DPRR-abs.py`: Drawing a violin plot based on the absolute value of the DPRR results.

#### Figure6c

- `Figure6c-heatmap-D-DPRR.py`: Drawing a heatmap plot based on D-DPRR results calculated by "D-DPRR.py".
