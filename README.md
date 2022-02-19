# LAGOS FOOD PRICES
Of the 36 states in Nigeria today, Lagos is considered to be one of the most expensive states to live in. This is because Lagos is the commercial hub of Nigeria, attracting numerous top-notch organizations. Hence, this has led to massive development in the state and subsequently a higher cost of living.



Food is any nutritious substance that people eat or drink to maintain life and growth. Food is essential to our everyday life, The high cost of living in Lagos has led to an increase in the prices of food. 
We will be analyzing the Selected food prices data (December 2021) gotten from the National Bureau of Statistics (https://nigerianstat.gov.ng/elibrary/read/1241108) to understand the changes in prices of rice on a month-on-month basis and year-on-year.  
Our focus on this research will be rice because rice is easily the most sought after food in Lagos and Nigeria in general.



The dataset contains the prices of 43 selected food items across the 36 states in Nigeria. We will be extracting the data for Lagos alone since our analysis is based on the changes in rice prices in Lagos.
Four different rice species are included in this data:
1. Rice agric sold loose
2. Rice local sold loose
3. Rice Medium Grained
4. Rice,imported high quality sold loose

![image](https://user-images.githubusercontent.com/98736158/154783711-aa484c6b-255a-421c-9c60-5942c4d9834c.png)



In this study, we are going to answer questions like: 
1. Did rice record a higher or lower price on a month-on-month basis and year-on-year basis?
2. What is the percentage of increase and decrease in rice prices on a month-on-month basis and year-on-year basis?
3. Is rice more expensive in Lagos?



This project was carried out using MySQL Workbench, Jupyter notebook, PowerBi and Microsoft Excel spreadsheet. The main languages used in this project are SQL and Python.



# STEP 1 - CLEANING AND PREPROCESSING THE DATA



N.B All the data used in this research is included in the dataset file.



We began this research by extracting the Data for Lagos state alone from the Selected food prices data (December 2021) gotten from the National Bureau of Statistics.


id	ItemLabels	17-Jan	17-Feb	17-Mar	17-Apr	17-May	17-Jun	17-Jul	17-Aug	17-Sep	17-Oct	17-Nov	17-Dec	18-Jan	18-Feb	18-Mar	18-Apr	18-May	18-Jun	18-Jul	18-Aug	18-Sep	18-Oct	18-Nov	18-Dec	19-Jan	19-Feb	19-Mar	19-Apr	19-May	19-Jun	19-Jul	19-Aug	19-Sep	19-Oct	19-Nov	19-Dec	20-Jan	20-Feb	20-Mar	20-Apr	20-May	20-Jun	20-Jul	20-Aug	20-Sep	20-Oct	20-Nov	20-Dec	21-Jan	21-Feb	21-Mar	21-Apr	21-May	21-Jun	21-Jul	21-Aug	21-Sep	21-Oct	21-Nov	21-Dec
1	Agric eggs medium size	597	591.82	586.32	526.32	528.42	526.5	468.24	492.63	473.68	461.25	459.41	473.89	400	490.53	512.77	482.38	462.35	496.92	477.04	503.81	469.21	468.1	447	475	461.58	445.88	448.7	439.44	440	495.26	468.13	467.3	465.25	465.71	492.11	454.5	451.36	465.26	480.75	565.71	498.1	500	517.5	520	557	563.75	531	537.22	548.5	539.12	553.18	568.1	580	611.5	676.5	692.5	700	735	740.06	763.33
2	Agric eggs(medium size price of one)	50.74	54.14	51.05	49.41	49.28	45.43	40.88	41.18	40.31	40.15	41.51	40.94	35	40.79	40.65	39.05	41.14	39.23	40.19	42.57	40.26	41.75	42.5	42.25	40	39.71	40.65	39.41	40.48	39.21	39.89	40.55	40.53	38.5	41.58	42.35	39.09	39.47	40.67	47.32	42.48	42.67	43.5	45.33	44.5	47.56	45.5	45	48	47.37	50.38	50.57	51.67	51.58	62	58.13	66.47	68	70	73.18
3	Beans brown,sold loose	416.7	418.1	395.17	358.96	388.76	412.53	424.56	488.13	484.87	480.76	472.79	417.56	417.56	420.5	455.47	461.71	400	457.55	495.9	467.76	498.74	494.23	466.09	468.12	467.45	393.38	376.83	374.31	343.48	310.6	269.84	265.13	270.49	268.13	263.63	259.69	287.6	255.56	253.05	299.92	268.48	295.07	295.63	290.76	296.94	296.82	272.64	292.01	301.21	342.16	347.67	346.16	358.88	342.38	388.29	484.88	481.76	438.56	440.54	449.63
4	Beans:white black eye. sold loose	364.85	354.73	356.56	348.42	386.97	411.22	409.92	402.11	406.27	395.79	395.79	404.78	450	409.8	453.27	441.54	526.36	530.75	443.56	446.56	455.31	400.92	400.58	443.58	440	398.29	386.9	369.64	391.98	307.04	272.94	306.57	315.23	296.14	282.71	299.92	306.66	295.75	304.43	300.42	296.04	305.41	319.67	310.29	326.83	330.17	343.59	359.47	370.36	363.94	343.28	356.32	396.32	386.9	372.81	471.73	497.47	499.63	500.86	511.18
5	Beef Bone in	1008.16	1025.56	1124.77	1055.56	1132.64	1169.07	1111.11	1122.83	1192.13	1129.17	1151.19	1525.93	1525.93	1314.46	1126.19	1090.74	1500	1320.59	1256.79	1230	1172.22	1110.56	1024.07	1122.13	1223.81	1130.77	1126.51	1155.4	1145.59	1163.64	1149.43	1095.25	1129.36	1120.47	1160.8	1175.19	1148.74	1188.26	1223.54	1294.67	1288.19	1283.54	1243.31	1205.43	1254.91	1213.5	1229.86	1222.97	1236.36	1283.33	1302.38	1325.44	1343.39	1349.57	1367.76	1393.33	1430.91	1500.27	1500.72	1520.81
6	Beef,boneless	1363.31	1378.88	1320.91	1264.91	1404.39	1472.63	1451.51	1673.78	1640.57	1633.33	1691.18	1689.19	1389.19	1207.18	1238.76	1250.97	1344.02	1324.71	1326.05	1522.5	1325.13	1266.67	1319.05	1264.11	1312.55	1284.8	1267.46	1248.77	1211.5	1264.04	1241.42	1275.92	1306.84	1276.55	1329.48	1318.34	1329.15	1230.59	1282.17	1374.92	1322.51	1350.46	1364.77	1354.43	1335.65	1369.25	1399.4	1373.85	1341.81	1308.9	1358.04	1376.79	1327.78	1398.74	1466.91	1569.44	1625.2	1664.26	1678.65	1700
7	Bread sliced 500g	308.05	304	299.52	289.47	294.21	307.62	291.18	272.22	266.67	258.46	250.24	309.38	350	328.21	339.52	297.62	295.56	296.32	305.17	295	297.37	295.71	305	306.5	308.82	291.67	274.76	287.78	288.64	205.26	247.89	298.21	288.89	292.96	290.56	295.24	288.1	288.89	295.83	325	325	311.5	316.5	318.13	323.33	330.63	335.26	344.44	344.44	352.94	360	376.32	397.06	365.79	397.37	425	402.94	434.21	412.5	428.5
8	Bread unsliced 500g	265.81	256.39	259	253.89	260	250	238	267.5	272.22	265	256.25	250	300	252.78	298.81	252.27	262.96	241.3	256.07	247.62	252.63	243.18	252.5	238.1	257.49	255.56	254.55	263.16	275	247.22	255.56	250	245	242.22	244.74	259.52	252.38	260.53	253.57	300	282.5	286.67	286.67	278.95	279.53	278.82	272.78	286.11	315.29	326.88	322.73	315	322.22	344.76	352.63	363.33	398.75	395	408.33	379.55
9	Broken Rice (Ofada)	720.61	712.3	709.26	705.56	699.4	698.09	689.31	566.34	562.3	548.27	548.27	575.86	641.67	588.69	566.58	578.24	602.58	661.46	610.54	578.69	539.13	522.22	608.96	581.05	540	557.42	540.89	530.01	510.52	534.05	516.48	523.57	543.01	504.6	526.97	551.59	548.46	585.98	612.9	644.14	615.4	639.32	677.95	641.85	690.03	710.65	761.77	810.19	851.49	821.89	827.45	898.61	938.61	825.52	844.13	844.36	849.66	869.28	842.5	850.25
10	Chicken Feet	998.83	970	950	916.67	1025	1100	1140	1066.67	1067.2	1000	940	1141.67	1141.67	925	875.57	792.86	811.8	875	1036.36	970	1033.33	900	850	850	916.61	828.57	833.33	850	820	800	780	812.5	784	720.21	700	726.67	704.08	720	755	820	742.86	766.67	812.5	816.67	826.67	833.33	828.57	840	858.57	888.75	926.36	966.67	943.75	955	980	987.5	997.43	1055.56	1060.33	1060.33
11	Chicken Wings	1079.07	1098.21	1028.57	1062.13	1065.63	1117.65	1190	1200	1200.6	1113.89	1076.47	1164.71	1164.71	1082.5	1143.48	1010	1125.96	1129.55	1177.78	1131.58	1134.21	1147.5	1155.56	1157.89	1129.21	1028.57	1009.52	1163.16	1125.45	1057.89	1012.63	1026.78	1005.9	964.29	1003.33	1006.67	1002.5	1051.67	1076.92	1127.78	1117.59	1105.26	1126.47	1190.63	1172.38	1189.41	1135	1126.47	1157.5	1189.47	1190.48	1168.42	1164.71	1170	1200	1237.5	1378.57	1421.05	1526.11	1604.76
12	Evaporated tinned milk carnation 170g	140.02	126.67	140	150	152.86	156.67	178.75	156	170	155.71	155.71	145	160	153.33	152.27	158	157.64	153.33	150	147.5	151.67	145	142.5	155	152.1	151.67	148.57	151.43	157.5	146.67	150	158	152.5	150	150	150	155.71	150	150	182.73	172.86	176	186.67	180	186.67	182.86	184	180	180	187.5	185.71	231.25	192	194.29	205.71	219.67	220	227.5	216.67	240
13	Evaporated tinned milk(peak), 170g	145	173.36	192	196.11	195.71	197.14	195.29	210	206.18	198.67	198.67	197.22	198	190.59	190.17	195.16	205	193.91	200.5	198.38	202.11	201	200.5	200.15	220	208.13	200.95	203.16	203.81	195.88	182.63	205.38	200.89	192.94	198.94	196.19	195	196.11	197.33	204.25	202.22	202.38	206.84	210	209.5	210.67	212	201.67	211.67	218.89	216.36	234.21	220	238.57	241	248.67	250.59	248.95	268.89	279.39
14	Frozen chicken	1172.56	1290.97	1244.44	1378.95	1357.89	1438.1	1466.67	1331.58	1340	1232.35	1318.75	1293.75	1293.75	1310.53	1304.17	1240	1325.68	1264.58	1303.45	1245	1278.95	1295	1263.16	1276.19	1283.12	1304.67	1316.84	1488.24	1467.65	1500	1505.26	1509.28	1630	1671.43	1650	1679.41	1650	1629.41	1621.43	1684.29	1625	1680	1677.78	1700	1678.95	1687.14	1757.89	1800	1775.26	1822.22	1868.18	1818.75	1900	1988.89	2061.11	2085.71	2196.88	2215.79	2387.5	2451.9
15	Gari white,sold loose	208.1	270.37	304.94	280.03	282.7	317.6	319.9	334.96	319.95	297.32	241.76	200.71	200	237.75	204.74	200.66	225.94	206.88	195.07	204.8	183.88	151.45	130.36	129.53	136.01	138.16	127.43	134.58	131.29	123.34	143.93	136.91	139	132.09	128.51	126.59	154.81	145.71	140.45	171.62	156.67	161.72	173.59	162.15	170.9	170.18	176.56	253.21	262.42	261.49	306.89	347.37	356.7	360.21	344.96	340.02	358.4	356.15	372.89	374.93
16	Gari yellow,sold loose	264.82	267.65	317.41	302.72	313.43	347.77	366.57	370.38	374.52	339.44	307.15	240.91	235	266	245.56	241.18	299.23	314.88	317.15	334.34	334.34	298.44	253.88	185.89	196.43	165.5	151.11	157.5	161.65	138.04	147.13	152.18	168.35	160.12	161.65	150.81	189.86	180.07	190.85	203.43	197.23	207.59	205.13	206.72	207.94	202.23	200.32	235.18	272.07	275.8	277.17	312.79	363.29	366.21	367.85	368.24	390.29	399.31	481.98	490.56
17	Mudfish (aro) fresh	1132.35	1480.63	1313.64	1088.89	1050	1057.52	1180	1162.5	1157.14	1086.36	1039.17	1246.43	1246.43	1379.17	1402.94	1286.67	1285.37	1109.38	1190.48	1216.05	1100	1122.73	1135.71	1028.57	1120	1086.36	1066.67	1072.5	1045.45	984.43	962.5	1013.33	985.69	956.67	1012.31	1018.46	1086.67	1060.71	1098.89	1162.96	1134.82	1178.96	1186.36	1150	1131.82	1148.04	1167.42	1212.5	1156.67	1172.22	1180	1150	1219.85	1222.73	1321.43	1470	1437.48	1451.62	1577.78	1617.46
18	Mudfish : dried	2475.72	2169.01	2206	2215.99	2331.72	2204.17	2405.77	2464.29	2483.33	2238.89	2388.89	2175	2175	1850	1830.61	1917.86	2093.91	2000.79	2200	1991.67	2152.38	2130	2287.5	2168.1	2061.65	2027.38	1998.6	1957.14	1899.29	1808.61	1781.43	1804.28	1792.86	1725.24	1781.43	1821.43	1781.44	1768.73	1798.78	1819.17	1808.71	1806.29	1814.29	1891.43	1826.3	1859.52	1784.05	1740.91	1800.61	1794.9	1837.72	1906.21	1833.33	1764.29	1850.71	2025.87	2170.22	2203.57	2327.14	2378.57
19	Onion bulb	294.95	315.8	322.45	285.21	287.3	294.36	283.69	397.35	322.44	310.01	299.71	314.95	300	294.9	232.2	301.09	301.15	353.82	350.57	347.97	355.25	354.77	368.89	266.15	233.33	245.22	232.76	242.11	216.84	209.98	213.48	259.28	254.86	202.06	249.19	264.7	217.84	221.31	278.91	272.57	248.74	274.72	278.04	272.23	289.39	298.62	249.61	224.09	217.22	231.25	234.02	280.39	313.02	342.25	431.19	444.8	419.28	463.56	500.3	609.37
20	Rice agric sold loose	298.78	429.57	392.51	369.78	379.26	376.03	363.02	337.75	336.16	318.73	315.24	320.43	310	305.79	288.37	307.57	328.71	313.2	318.35	314.09	293.59	301.62	316.77	315.02	309.24	307.92	298.16	309.22	309.82	347.3	322.04	318.2	341.65	317.13	352.74	367.11	361.33	349.51	367.46	415.46	412.84	419.66	425.2	421.15	425.79	436.96	470.97	439.64	427.12	444.85	420.66	424.98	434.13	464.05	480.21	507.34	470.29	479.48	509.1	555.81
21	Rice local sold loose	321.03	359.37	344.44	345	391.67	400	399.5	367.98	372.5	295.23	295.23	342.66	330	350.22	298.66	266.67	309.67	296.88	290	304.84	297.18	300	300.67	334.52	335.88	320	300	312.02	292.16	259.46	300	323.52	355.23	375	409.27	419.27	401.79	422.72	389.52	414.51	418.31	423.67	426.63	439.83	440.83	448.53	449.08	443.12	414.94	426.67	416.7	406.52	434.57	418.27	405.76	426.25	432.67	444.55	445.67	503.15
22	Rice Medium Grained	280.82	340.33	322.12	322.58	330.12	336.35	317.54	324.25	336.77	336.77	336.77	296.77	295.36	295.36	292.58	308.26	316.74	323.53	322.58	322.58	322.9	312.02	319.16	330.97	335.26	312.05	300.25	311.95	309.68	309.68	281.25	295.12	311.02	325.01	325.5	325.5	330.15	312.52	350	363.33	354.19	355.5	361.61	351.61	359.14	378.38	373.12	375	385	371.61	385.45	345.16	349.35	442	506.67	515	521	525	600	600
23	Rice,imported high quality sold loose	402.54	417.94	386.96	329.84	370.33	371.2	383.14	319.24	344.76	314.07	309.81	306.87	306.87	311.08	319.39	296.39	318.24	315.96	330.06	338.55	388.79	370.99	308.71	334.19	322.58	305.96	301.65	333.95	335.2	342.54	320.37	318.03	324.92	374.39	358.63	361.38	391.09	381.85	407.24	482.64	492.53	509.56	527.83	527.7	529.03	536.83	547.98	539.24	577.89	572.79	536.24	595.65	563.67	661.72	604.08	607.36	610.95	629.32	663.59	697.66
24	Tomato	300	534.61	456.36	450	522.49	527.64	566.98	587.27	450.91	420.67	388.25	415.05	400	401.92	400.44	530.18	560	565.41	592.51	523.11	575.92	407.15	436.25	384.91	466.67	340.66	335.15	322.71	301.23	256.27	289.37	289.93	282.54	208.91	239.09	243.95	208.65	233.75	259.42	282.11	294.1	315.44	300	282.43	294.19	297.01	287.52	266.39	223.1	267.9	230.12	301.15	309.72	335.64	370.9	376.44	331	356.44	428.01	554.76
25	Yam tuber	209.06	216.46	221.47	233.42	297.7	302.36	303.43	312.87	258.48	210.03	210.16	207.62	200	201	232.5	390.31	408.33	463.79	437.72	430.34	415.3	395.77	279.32	230.97	234.83	222.92	215.79	262.85	285.73	243	203.65	245.8	221.95	206.79	257.35	243.9	214.71	223.74	221.71	242.17	242.51	256.79	285.24	292.66	277.47	275.17	293.95	283.44	309.1	292.56	303.5	316.56	316.71	342.63	407.39	467.18	464.87	476.78	600.27	623.02
26	Dried Fish Sardine	1998.22	1976.39	1921.17	1921.48	1993.36	1981.11	1993.06	1924.07	1890.34	1764.7	1802.78	1625	1520	1322.45	1301.02	1350	1384.64	1396.96	1395.9	1401.74	1411.11	1477.22	1476.56	1545.45	1413.4	1410.62	1416.36	1500.49	1463.94	1377.78	1349.05	1325.13	1346.91	1293.06	1198.5	1172.7	1248.53	1228.57	1216.67	1235.67	1229.23	1241.27	1224.07	1236.11	1237.5	1202.22	1176.27	1187.41	1165.28	1165.67	1112.5	1105.56	1183.33	1258.25	1319.5	1304.44	1355.7	1400	1278.41	1383.33
27	Iced Sardine	820.8	817.02	814.21	828.89	828.82	813.12	831.25	848.42	842.46	813.44	859.43	887.5	887.5	997.78	837.5	887.5	859.93	861.51	960.14	991.25	932.97	920.36	835.48	833.33	898.66	886.61	878.46	875.44	858.97	795.56	821.54	857.49	878.79	903.6	973.5	1005.65	983.61	983.02	960	1013.6	977.02	985.99	987.37	959.17	945.43	932.69	973.28	938.53	997.44	992.5	980	942.47	961.11	1019.23	1035.9	1251.28	1233.61	1233.33	1300	1375
28	Irish potato	326.94	320.42	325.64	321.98	320.2	328.92	327.52	335.12	330.27	360.78	351.85	399.11	350	330.71	325.04	339.82	377.78	389.37	405	378.7	401.78	385.27	371.76	292.26	310	314.16	315.22	328.76	307.04	371.65	350.54	402	393.81	349.18	362.24	377.08	308.31	367.86	400.95	480.92	457.22	490.13	496.4	456.26	457.57	473.23	444.93	476.36	506.79	572.88	481.99	473.22	471.22	520.43	570.56	518.93	525.94	553.98	632.37	843.02
29	Sweet potato	137.91	135.68	138.25	138.97	139.04	144.97	146.52	148.18	148.49	102.59	106.22	125.5	125	135	148.51	157.96	164.54	175.74	197.27	198.77	201.53	221.82	218.41	201.76	217.02	212.73	193.66	189.24	250.65	209.74	170.62	200.03	163.97	139.27	201.02	226.36	181.97	196.5	206.56	219.98	204.42	208.19	226.65	229.39	228.76	238.16	231.57	226.06	207.2	225.43	236.76	232.66	235.96	268.53	268.99	241.2	246.65	269.27	246.19	350.44
30	Tilapia fish (epiya) fresh	864.48	949.4	956.95	942.13	938.57	1012.15	1057.74	1038.2	1066.67	1187.12	1187.12	1145.45	1145.45	1167.26	1185.77	1214.29	1218.93	1161.11	1208.7	1216.67	1293.75	1156.25	1187.5	1062.5	1183.65	985.71	983.33	971.43	910.53	850	797.59	808.69	810.79	777.78	805.98	823.33	827.21	828.13	876.67	932.25	873.33	861.54	887.69	896.15	963.64	996.67	996.59	1006.1	1013.33	1043.75	1094.51	1034.14	1058.33	1168.75	1213.33	1450.35	1528.57	1594.44	1730.77	1844.44
31	Titus:frozen	929.5	933.64	972.92	931.68	981.68	1063.57	1058.89	1051.11	999.41	1010.43	1061.76	1038.24	1038.24	1018.42	947.83	984.21	1020.52	986.43	970.37	971.43	981.58	935	945	991.67	982.09	940.63	930	952.78	922.22	984.21	921.94	978.57	983.33	968.42	981.58	1018.42	947.73	936.84	989.29	1007.69	998.1	998.05	1008.95	1007.06	1009	1072.22	1035	1058.89	1082.5	1065.93	1021.74	1109.52	1131.58	1238.11	1354.47	1326.67	1433.98	1473.64	1530.3	1590.91
32	Catfish (obokun) fresh	1239.16	1297.93	1259.55	1332.69	1394.2	1390.84	1395.04	1396.7	1381.66	1417.7	1303.92	1400.65	1400.65	1358.25	1291.67	1165.03	1256.14	1271.97	1300.75	1312.7	1356.21	1439.55	1396.5	1354.79	1396.17	1305.56	1318.62	1394.44	1381.88	1297.37	1285.43	1308.05	1287.04	1282.46	1270.59	1288.24	1265.48	1224.38	1270.69	1323.22	1297.46	1311.88	1342.67	1387.86	1364.88	1358.5	1396.08	1399.4	1369.92	1396.22	1394.78	1381.25	1364.74	1408.33	1460.71	1652.38	1767.08	1784.44	1821.2	1856.99
33	Catfish :dried	2252.65	2300.35	2369.82	2359.63	2365.06	2404.51	2400.69	2400	2385.84	1982.96	2178.66	2193.22	2193.22	1950	1908.89	1807.69	1827.48	1891.67	1852.86	1854.03	1505.88	1546.67	1537.59	1643.37	1782.87	1800	1797.5	1730	1729.17	1653.13	1596.48	1611.64	1614.17	1586.26	1597.73	1617.42	1568.61	1562.5	1606.99	1666.55	1620.2	1689.9	1751.79	1790	1760.36	1786.67	1710.32	1712.59	1760.78	1707.65	1722.73	1745.03	1798.4	1752.38	1845.24	2060	2061.04	2089.01	2218.18	2346.1
34	Catfish Smoked	1554.26	1576.92	1575	1509.26	1500.5	1513.64	1522.3	1526.37	1514.37	1500	1533.33	1534.09	1534.09	1525	1500	1500	1500	1511.75	1600	1671.98	1640	1500	1567.44	1700	1560.99	1600	1595	1633.33	1670	1593.33	1582.61	1600	1577.78	1554.76	1550	1575	1542.22	1560	1594.29	1607.58	1585.71	1600	1641.07	1546.94	1576.19	1562.65	1572.32	1540	1538.66	1591.67	1633.33	1675	1687.14	1686.8	1778.61	1889.47	1812.38	1830	1850.79	1850.79
35	Mackerel : frozen	1030.19	993.01	987.5	1067.59	1049.43	1051.37	1094.03	1065.34	1065.45	1083.33	1087.06	975	975	960	1029.55	918	1027.93	980.95	927.16	963.02	948.33	827.82	826.32	888.33	907.16	940.63	931.48	947.37	892.73	848.32	803.79	836.66	901.5	925	888.64	903.23	847.62	886.11	929.94	1012.36	936.16	992.5	1011.4	1016.67	1089.61	1014.71	1075.79	1057.63	1063.13	1000	1064.71	1095	1121.05	1227.21	1236.92	1225	1284.06	1233.06	1296.88	1280.95
36	Groundnut oil: 1 bottle, specify bottle	483.3	486.66	492.22	500	504.13	484.44	480	500	490.36	485.16	485.16	506.67	500	500	666.67	550	560.62	606.67	533.33	602.22	583.33	550	533.33	483.33	553.57	533.33	513.33	517.78	500	544.44	533.33	500	533.33	513.33	533.33	546.67	533.33	540	540	600	586.67	600	600	600	577.78	588.89	533.33	533.33	566.67	545	533.33	583.33	580	653.34	726.67	833.33	966.67	971.11	996	1066.67
37	Maize grain white sold loose	222.99	219.01	224.22	236.16	242.02	244.87	269.29	244.56	208.39	245.23	245.23	222.33	225	283.82	214.86	232.52	238.98	250.42	250.46	211.33	215.43	198.61	227.14	209.64	228.81	219.11	200.51	214.99	207.05	222.88	202.49	199.01	206.92	208.91	224.2	204.97	246.57	252.01	247.37	251.73	250.82	240.05	269.18	238.83	235.94	261.7	273.21	257.27	274.48	263.77	302.49	312.43	356.2	359.21	340.2	356.66	362.59	326.49	400	557.43
38	Maize grain yellow sold loose	221.35	232.54	224.85	242.8	245.88	252.72	279.65	263.04	219.42	253.09	253.09	229.15	250	280.42	247.13	239.88	250.54	255.37	224.45	218.21	213.44	211.97	228	200.56	233.99	241.19	221.81	218.75	206.63	230.29	207.3	201.76	204.14	204.05	233.65	210.59	254.51	245.65	242.13	258.9	256.3	243.82	274.42	273.31	286.7	268.52	273.63	259.42	252.99	267.37	265.03	278.88	358.22	365.58	349.19	370.48	348.53	343.78	450	403.18
39	Palm oil: 1 bottle,specify bottle	410.5	423.56	472.48	508.85	500	518.52	523.8	550	559.32	559.29	559.29	537.25	466.67	519.3	490.91	450	455.56	500	482.67	501.75	505.26	498.04	501.75	516.08	444.44	412.35	403.94	462.96	473.02	447.72	440	475.06	480	466.67	480.7	514.81	496.3	486.27	461.9	489.73	483.33	504.67	503.33	510.83	516.67	532.55	662.96	681.48	656.67	668.07	654.55	673.33	679.82	720.64	810	831.11	811.76	851.33	977.78	985.34
40	Plantain(ripe)	302.21	300	287.36	261.97	243.92	255.28	276.84	234.5	256.89	255.66	241.13	210.67	230	210	218.67	246.28	259.2	240.24	222.75	229.31	218.43	178.41	182.57	229.67	220.92	198.82	195.66	277.6	223.99	207.08	241.53	236.36	205.31	249.01	249.41	231.72	236.42	233.41	279.85	311.88	282.07	245.62	258.71	283.74	367.83	343.29	375.22	341.33	309.84	384.05	394.5	390.39	388.61	391.81	379.22	364.42	411.38	356.19	367.5	381.31
41	Plantain(unripe)	307.14	284.35	283.09	292.2	283.11	286.05	270.61	256.92	284.83	286.47	267.87	246.42	224.14	208.54	196.22	187.99	203.66	190.48	205.04	198.79	205.02	166.25	162.87	201.17	195.12	205.39	197.72	276.74	242.47	202.28	251.27	216.38	188.6	234.39	251.32	286.86	236.1	231.48	280.67	316.06	291.51	264.2	261.29	259.17	305.38	293.94	303.1	291.09	270.82	288.26	291.81	301.47	389.01	410.15	354.03	348.72	331.42	359.61	382.93	401.2
42	Vegetable oil:1 bottle,specify bottle	598.42	507.26	538.18	552.81	559.14	550	555.55	578.57	555.3	550.82	550.82	533.33	550	554	528.67	528.67	566.67	530.3	523.08	522.81	537.04	509.8	529.63	511.11	532.4	500.17	488.07	509.8	533.33	519.3	520.63	533.33	540	530.16	568.42	563.7	557.89	546.67	552.38	590.99	590.48	581.48	585.44	620.51	627.41	630.7	723.33	757.78	753.33	784.81	715.87	748.15	755.56	836.67	918.89	930.48	925.93	950	1025	1078.21
43	Wheat flour: prepacked (golden penny 2kg)	636.66	666.27	631.25	625.79	622.55	639.04	639.44	644.09	602.52	639.99	640	648.75	648.75	620.59	641.75	609.47	632.9	619.05	610.37	594.74	572.5	616.5	590	582.5	611.18	621.88	625.27	594.74	606.82	601.67	600	607.69	595.24	615	627.5	588.1	585.43	586.88	645.83	670	671.43	669.44	673.75	700	698.56	692.41	696	653.89	701.18	691.18	707.5	730.56	776.47	765.79	819.44	870	900	950	980	995
![image](https://user-images.githubusercontent.com/98736158/154784113-3b4a418f-aae2-4131-9b21-76c9fa3955f6.png)
