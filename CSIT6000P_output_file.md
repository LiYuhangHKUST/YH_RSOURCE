## **CSIT6000P Spatial and Multimedia Databases**

# Assignment 1 Output

###### Task 1 Outputs:

```
Task 1 [5 marks] (MBR calculation)
    (1) [1 mark] Write a program to compute the spatial extent of dataset D. The spatial extent of D is the MBR of all polygons in D. Report the MBR of D.
        Spatial extent of dataset D:  (113.9310037, 22.1973011, 114.3763554, 22.5069962)
    (2) [2 marks] Create dataset D’ which adds an MBR column for the polygon in each record in D' Output the spreadsheet file for the new dataset D’.
        Output the spreadsheet file for the new dataset D’ is store as: Buildings_with_MBR.xlsx
    (3) [2 marks] Let n be the resolution for recursive decomposition of the space as defined by the spatial extent of D. What are the sizes (in cm by cm) of the smallest Peano cells for n = 12, 16 and 20 respectively? Show your calculation steps. Please also discuss which resolution value is suitable for D.
        The size of the smallest Peano cell for n = 12 is 1121.19 cm by 837.26 cm and area = 938728.40 cm^2.
        The size of the smallest Peano cell for n = 16 is 70.07 cm by 52.33 cm and area = 3666.91 cm^2.
        The size of the smallest Peano cell for n = 20 is 4.38 cm by 3.27 cm and area = 14.32 cm^2.
        Here are the calculation steps: 
        --------------------An ornate dividing line----------------------
        Calculation steps for n = 12:
            x_size = (114.3763554 - 113.9310037) * 111319.9 * 100 = 4592407.17 cm
            y_size = (22.5069962 - 22.1973011) * 111319.9 * 100 = 3429410.45 cm
            x_cell_size = x_size / 2 ** n = 4592407.17 / 2 ** 12 = 1121.19 cm
            y_cell_size = y_size / 2 ** n = 3429410.45 / 2 ** 12 = 837.26 cm
            Size of smallest Peano cell for n = 12: 1121.19 cm x 837.26 cm = 938728.40 cm^2

        Calculation steps for n = 16:
            x_size = (114.3763554 - 113.9310037) * 111319.9 * 100 = 4592407.17 cm
            y_size = (22.5069962 - 22.1973011) * 111319.9 * 100 = 3429410.45 cm
            x_cell_size = x_size / 2 ** n = 4592407.17 / 2 ** 16 = 70.07 cm
            y_cell_size = y_size / 2 ** n = 3429410.45 / 2 ** 16 = 52.33 cm
            Size of smallest Peano cell for n = 16: 70.07 cm x 52.33 cm = 3666.91 cm^2

        Calculation steps for n = 20:
            x_size = (114.3763554 - 113.9310037) * 111319.9 * 100 = 4592407.17 cm
            y_size = (22.5069962 - 22.1973011) * 111319.9 * 100 = 3429410.45 cm
            x_cell_size = x_size / 2 ** n = 4592407.17 / 2 ** 20 = 4.38 cm
            y_cell_size = y_size / 2 ** n = 3429410.45 / 2 ** 20 = 3.27 cm
            Size of smallest Peano cell for n = 20: 4.38 cm x 3.27 cm = 14.32 cm^2


Process finished with exit code 0
```

Task 2 Output:

```
Task 2 (1) Output the spreadsheet file with the new columns.
Output the spreadsheet file for the new dataset D’ is store as: Buildings_with_Z-value.xlsx
Task 2 (2) Output some random polygons:
Polygon index: 51633
MBR: POLYGON ((114.2663275 22.3216542, 114.2663275 22.321779, 114.2661887 22.321779, 114.2661887 22.3216542, 114.2663275 22.3216542))
Z-value 12: 22675042, Peano cell size (12): 1121.1935588297433 x 837.2424458505019 cm
Z-value 16: 9300018792, Peano cell size (16): 70.07459747265436 x 52.3276525890269 cm
Z-value 20: 44412376190667, Peano cell size (20): 4.379662387834799 x 3.270478273201137 cm
Best resolution for polygon 51633: 20

Polygon index: 17752
MBR: POLYGON ((114.1698992 22.3064119, 114.1698992 22.3064813, 114.1697582 22.3064813, 114.1697582 22.3064119, 114.1698992 22.3064119))
Z-value 12: 175955132, Peano cell size (12): 1121.1935588297433 x 837.2424458505019 cm
Z-value 16: 45830252007, Peano cell size (16): 70.07459747265436 x 52.3276525890269 cm
Z-value 20: 42770439627007, Peano cell size (20): 4.379662387834799 x 3.270478273201137 cm
Best resolution for polygon 17752: 20

Polygon index: 31927
MBR: POLYGON ((114.161353 22.4481826, 114.161353 22.4482146, 114.1613279 22.4482146, 114.1613279 22.4481826, 114.161353 22.4481826))
Z-value 12: 35260008, Peano cell size (12): 1121.1935588297433 x 837.2424458505019 cm
Z-value 16: 69615338133, Peano cell size (16): 70.07459747265436 x 52.3276525890269 cm
Z-value 20: 51186558697508, Peano cell size (20): 4.379662387834799 x 3.270478273201137 cm
Best resolution for polygon 31927: 20

Polygon index: 4859
MBR: POLYGON ((114.1926191 22.3860621, 114.1926191 22.3867885, 114.1917431 22.3867885, 114.1917431 22.3860621, 114.1926191 22.3860621))
Z-value 12: 24385378, Peano cell size (12): 1121.1935588297433 x 837.2424458505019 cm
Z-value 16: 61303682253, Peano cell size (16): 70.07459747265436 x 52.3276525890269 cm
Z-value 20: 20813256807253, Peano cell size (20): 4.379662387834799 x 3.270478273201137 cm
Best resolution for polygon 4859: 20

Polygon index: 35894
MBR: POLYGON ((114.123021 22.44058, 114.123021 22.4406463, 114.1229612 22.4406463, 114.1229612 22.44058, 114.123021 22.44058))
Z-value 12: 150508191, Peano cell size (12): 1121.1935588297433 x 837.2424458505019 cm
Z-value 16: 106595820691, Peano cell size (16): 70.07459747265436 x 52.3276525890269 cm
Z-value 20: 58395170039441, Peano cell size (20): 4.379662387834799 x 3.270478273201137 cm
Best resolution for polygon 35894: 20


Process finished with exit code 0
```

Task 3 Output:

```
Task 3 (1) [7 marks] Write a program to perform window queries using two approaches: (i) by exhaustively checking every object in the dataset; and (ii) by using z-values you generate in Task 2 for the above three n values.
Example qurey: Q = {(113.9310037, 22.1973011), (114.3763554, 22.5069962)}
Exhaustive window query count: 76718
Z-value window query count (n=12): 76718
Z-value window query count (n=16): 76718
Z-value window query count (n=20): 76718
Enter your query as example format:Q = {(113.5, 22.1), (114.4, 22.2)}
Exhaustive window query count: 25
Z-value window query count (n=12): 25
Z-value window query count (n=16): 25
Z-value window query count (n=20): 25

Task 3 (2) [3 mark] Use 20 randomly generated window queries of different sizes at different locations to search using the programs you developed above, to report (i) the number of objects inside each query window, (ii) the number of objects searched for each query for using no z-values (i.e., exhaustive search) and using z-values obtained using different resolution numbers.
Query 1:
  Query window: minx    113.959532
miny     22.466502
maxx    114.128010
maxy     22.505156
Name: 0, dtype: float64
  Exhaustive window query count: 4781
  Z-value window query count (n=12): 4781
  Z-value window query count (n=16): 4781
  Z-value window query count (n=20): 4781


Query 2:
  Query window: minx    114.051171
miny     22.252693
maxx    114.204384
maxy     22.433594
Name: 0, dtype: float64
  Exhaustive window query count: 31610
  Z-value window query count (n=12): 31610
  Z-value window query count (n=16): 31610
  Z-value window query count (n=20): 31610


Query 3:
  Query window: minx    114.244049
miny     22.459600
maxx    114.263406
maxy     22.463509
Name: 0, dtype: float64
  Exhaustive window query count: 0
  Z-value window query count (n=12): 0
  Z-value window query count (n=16): 0
  Z-value window query count (n=20): 0


Query 4:
  Query window: minx    114.060370
miny     22.361437
maxx    114.163691
maxy     22.372544
Name: 0, dtype: float64
  Exhaustive window query count: 2105
  Z-value window query count (n=12): 2105
  Z-value window query count (n=16): 2105
  Z-value window query count (n=20): 2105


Query 5:
  Query window: minx    114.071286
miny     22.349148
maxx    114.294055
maxy     22.436358
Name: 0, dtype: float64
  Exhaustive window query count: 15653
  Z-value window query count (n=12): 15653
  Z-value window query count (n=16): 15653
  Z-value window query count (n=20): 15653


Query 6:
  Query window: minx    114.278657
miny     22.372394
maxx    114.282133
maxy     22.467612
Name: 0, dtype: float64
  Exhaustive window query count: 2
  Z-value window query count (n=12): 2
  Z-value window query count (n=16): 2
  Z-value window query count (n=20): 2


Query 7:
  Query window: minx    114.034213
miny     22.296404
maxx    114.290774
maxy     22.367660
Name: 0, dtype: float64
  Exhaustive window query count: 22760
  Z-value window query count (n=12): 22760
  Z-value window query count (n=16): 22760
  Z-value window query count (n=20): 22760


Query 8:
  Query window: minx    114.014187
miny     22.357414
maxx    114.351459
maxy     22.437405
Name: 0, dtype: float64
  Exhaustive window query count: 15673
  Z-value window query count (n=12): 15673
  Z-value window query count (n=16): 15673
  Z-value window query count (n=20): 15673


Query 9:
  Query window: minx    114.117671
miny     22.394527
maxx    114.170015
maxy     22.419358
Name: 0, dtype: float64
  Exhaustive window query count: 38
  Z-value window query count (n=12): 38
  Z-value window query count (n=16): 38
  Z-value window query count (n=20): 38


Query 10:
  Query window: minx    114.282208
miny     22.291427
maxx    114.288562
maxy     22.504865
Name: 0, dtype: float64
  Exhaustive window query count: 72
  Z-value window query count (n=12): 72
  Z-value window query count (n=16): 72
  Z-value window query count (n=20): 72


Query 11:
  Query window: minx    114.335362
miny     22.301652
maxx    114.367647
maxy     22.506623
Name: 0, dtype: float64
  Exhaustive window query count: 74
  Z-value window query count (n=12): 74
  Z-value window query count (n=16): 74
  Z-value window query count (n=20): 74


Query 12:
  Query window: minx    114.347138
miny     22.406080
maxx    114.366575
maxy     22.409559
Name: 0, dtype: float64
  Exhaustive window query count: 0
  Z-value window query count (n=12): 0
  Z-value window query count (n=16): 0
  Z-value window query count (n=20): 0


Query 13:
  Query window: minx    114.000470
miny     22.365836
maxx    114.361867
maxy     22.486961
Name: 0, dtype: float64
  Exhaustive window query count: 30935
  Z-value window query count (n=12): 30935
  Z-value window query count (n=16): 30935
  Z-value window query count (n=20): 30935


Query 14:
  Query window: minx    114.332199
miny     22.418292
maxx    114.341387
maxy     22.475974
Name: 0, dtype: float64
  Exhaustive window query count: 6
  Z-value window query count (n=12): 6
  Z-value window query count (n=16): 6
  Z-value window query count (n=20): 6


Query 15:
  Query window: minx    114.245839
miny     22.406384
maxx    114.292059
maxy     22.473937
Name: 0, dtype: float64
  Exhaustive window query count: 388
  Z-value window query count (n=12): 388
  Z-value window query count (n=16): 388
  Z-value window query count (n=20): 388


Query 16:
  Query window: minx    113.947574
miny     22.491743
maxx    114.369351
maxy     22.502342
Name: 0, dtype: float64
  Exhaustive window query count: 2796
  Z-value window query count (n=12): 2796
  Z-value window query count (n=16): 2796
  Z-value window query count (n=20): 2796


Query 17:
  Query window: minx    114.119418
miny     22.346202
maxx    114.237746
maxy     22.491356
Name: 0, dtype: float64
  Exhaustive window query count: 19560
  Z-value window query count (n=12): 19560
  Z-value window query count (n=16): 19560
  Z-value window query count (n=20): 19560


Query 18:
  Query window: minx    114.071895
miny     22.298858
maxx    114.361939
maxy     22.347694
Name: 0, dtype: float64
  Exhaustive window query count: 18676
  Z-value window query count (n=12): 18676
  Z-value window query count (n=16): 18676
  Z-value window query count (n=20): 18676


Query 19:
  Query window: minx    114.075328
miny     22.499114
maxx    114.088830
maxy     22.502720
Name: 0, dtype: float64
  Exhaustive window query count: 52
  Z-value window query count (n=12): 52
  Z-value window query count (n=16): 52
  Z-value window query count (n=20): 52


Query 20:
  Query window: minx    114.334582
miny     22.409422
maxx    114.342120
maxy     22.438004
Name: 0, dtype: float64
  Exhaustive window query count: 2
  Z-value window query count (n=12): 2
  Z-value window query count (n=16): 2
  Z-value window query count (n=20): 2



Process finished with exit code 0

```

