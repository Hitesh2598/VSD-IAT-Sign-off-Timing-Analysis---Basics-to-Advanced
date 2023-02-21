# VSD-IAT-Sign-off-Timing-Analysis---Basics-to-Advanced
# Table of contents
  1. Lab 1
  2. Lab 2
  3. Lab 3
  4. Lab 4
  5. Lab 5


## **LAB 1**




## **LAB 2**


Liberty File : The .lib file is an ASCII representation of the timing & power parameters associated with any cell in a particular semiconductor technology
                .lib file contains:-
								    1. Timing Models
										2. Data to calcumac
										       1. I/O delay paths
													 2.Timing check values
                           3.Interconnect delays
													 
Command for reading liberty file:-
       			
							read_liberty  
							

![lib file](https://user-images.githubusercontent.com/108817818/220392152-df7a686b-ceb2-4924-b1ca-599a0a99d2a8.jpg)
![lib2](https://user-images.githubusercontent.com/108817818/220392535-689aa0d4-fac6-4bcc-a001-380ce20ce80e.jpg)
![lib3](https://user-images.githubusercontent.com/108817818/220392638-e3d37aea-735b-4af2-bdab-835df52fea12.jpg)


Commands to see lab 2 files
  
	cd lab2
	ls
	
.lib files present in lab 2 folder:
	
![terminal pic](https://user-images.githubusercontent.com/108817818/220396232-5bf3041e-799c-4ae0-ad74-7be830153df8.jpg)

To open .lib file use following commands :-

       leafpad simple_min.lib  
	 
       leafpad simple_max.lib
	

![opening simplemax](https://user-images.githubusercontent.com/108817818/220399280-38dd3d6e-4691-44bd-ae1f-095948d239f5.jpg)


**Exercise 1:**

**1. Find all the cells in simple_max.lib.**

Total 211 Cells 
		
				
		  Command Used				     				 
					 grep -c "Begin cell" simple_max.lib
									 
						
									
![total cell](https://user-images.githubusercontent.com/108817818/220402203-e92d3a4d-e266-45ba-b589-1524d6aaab49.jpg)
![list cell](https://user-images.githubusercontent.com/108817818/220404070-9c9c3069-762c-4c96-aedf-f2f87d658814.jpg)
							
List of all the cells available
1.	INV_X1       
2.	INV_X2 
3.	INV_X3 
4.	INV_X4 
5.	INV_X6 
6.	INV_X8 
7.	INV_X10 
8.	INV_X20 
9.	INV_X40 
10.	INV_X80 
11.	INV_Y1 
12.	INV_Y2 
13.	INV_Y3 
14.	INV_Y4 
15.	INV_Y6 
16.	INV_Y8 
17.	INV_Y10 
18.	INV_Y20 
19.	INV_Y40 
20.	INV_Y80 
21.	INV_Z1 
22.	INV_Z2 
23.	INV_Z3 
24.	INV_Z4 
25.	INV_Z6 
26.	INV_Z8 
27.	INV_Z10 
28.	INV_Z20 
29.	INV_Z40 
30.	INV_Z80 
31.	NAND2_X1 
32.	NAND2_X2 
33.	NAND2_X3 
34.	NAND2_X4 
35.	NAND2_X6 
36.	NAND2_X8 
37.	NAND2_X10 
38.	NAND2_X20 
39.	NAND2_X40 
40.	NAND2_X80 
41.	NAND2_Y01 
42.	NAND2_Y02 
43.	NAND2_Y03 
44.	NAND2_Y04 
45.	NAND2_Y06 
46.	NAND2_Y08 
47.	NAND2_Y10 
48.	NAND2_Y20 
49.	NAND2_Y40 
50.	NAND2_Y80 
51.	NAND2_Z01 
52.	NAND2_Z02 
53.	NAND2_Z03 
54.	NAND2_Z04 
55.	NAND2_Z06 
56.	NAND2_Z08 
57.	NAND2_Z10 
58.	NAND2_Z20 
59.	NAND2_Z40 
60.	NAND2_Z80 
61.	NAND3_X1 
62.	NAND3_X2 
63.	NAND3_X3 
64.	NAND3_X4 
65.	NAND3_X6 
66.	NAND3_X8 
67.	NAND3_X10 
68.	NAND3_X20 
69.	NAND3_X40 
70.	NAND3_X80 
71.	NAND3_Y1 
72.	NAND3_Y2 
73.	NAND3_Y3 
74.	NAND3_Y4 
75.	NAND3_Y6 
76.	NAND3_Y8 
77.	NAND3_Y10 
78.	NAND3_Y20 
79.	NAND3_Y40 
80.	NAND3_Y80 
81.	NAND3_Z1 
82.	NAND3_Z2 
83.	NAND3_Z3 
84.	NAND3_Z4 
85.	NAND3_Z6 
86.	NAND3_Z8 
87.	NAND3_Z10 
88.	NAND3_Z20 
89.	NAND3_Z40 
90.	NAND3_Z80 
91.	NAND4_X1 
92.	NAND4_X2 
93.	NAND4_X3 
94.	NAND4_X4 
95.	NAND4_X6 
96.	NAND4_X8 
97.	NAND4_X10 
98.	NAND4_X20 
99.	NAND4_X40 
100.	NAND4_X80 
101.	NAND4_Y1 
102.	NAND4_Y2 
103.	NAND4_Y3 
104.	NAND4_Y4 
105.	NAND4_Y6 
106.	NAND4_Y8 
107.	NAND4_Y10 
108.	NAND4_Y20 
109.	NAND4_Y40 
110.	NAND4_Y80 
111.	NAND4_Z1 
112.	NAND4_Z2 
113.	NAND4_Z3 
114.	NAND4_Z4 
115.	NAND4_Z6 
116.	NAND4_Z8 
117.	NAND4_Z10 
118.	NAND4_Z20 
119.	NAND4_Z40 
120.	NAND4_Z80 
121.	NOR2_X1 
122.	NOR2_X2 
123.	NOR2_X3 
124.	NOR2_X4 
125.	NOR2_X6 
126.	NOR2_X8 
127.	NOR2_X10 
128.	NOR2_X20 
129.	NOR2_X40 
130.	NOR2_X80 
131.	NOR2_Y1 
132.	NOR2_Y2 
133.	NOR2_Y3 
134.	NOR2_Y4 
135.	NOR2_Y6 
136.	NOR2_Y8 
137.	NOR2_Y10 
138.	NOR2_Y20 
139.	NOR2_Y40 
140.	NOR2_Y80 
141.	NOR2_Z1 
142.	NOR2_Z2 
143.	NOR2_Z3 
144.	NOR2_Z4 
145.	NOR2_Z6 
146.	NOR2_Z8 
147.	NOR2_Z10 
148.	NOR2_Z20 
149.	NOR2_Z40 
150.	NOR2_Z80 
151.	NOR3_X1 
152.	NOR3_X2 
153.	NOR3_X3 
154.	NOR3_X4 
155.	NOR3_X6 
156.	NOR3_X8 
157.	NOR3_X10 
158.	NOR3_X20 
159.	NOR3_X40 
160.	NOR3_X80 
161.	NOR3_Y1 
162.	NOR3_Y2 
163.	NOR3_Y3 
164.	NOR3_Y4 
165.	NOR3_Y6 
166.	NOR3_Y8 
167.	NOR3_Y10 
168.	NOR3_Y20 
169.	NOR3_Y40 
170.	NOR3_Y80 
171.	NOR3_Z1 
172.	NOR3_Z2 
173.	NOR3_Z3 
174.	NOR3_Z4 
175.	NOR3_Z6 
176.	NOR3_Z8 
177.	NOR3_Z10 
178.	NOR3_Z20 
179.	NOR3_Z40 
180.	NOR3_Z80 
181.	NOR4_X1 
182.	NOR4_X2 
183.	NOR4_X3 
184.	NOR4_X4 
185.	NOR4_X6 
186.	NOR4_X8 
187.	NOR4_X10 
188.	NOR4_X20 
189.	NOR4_X40 
190.	NOR4_X80 
191.	NOR4_Y1 
192.	NOR4_Y2 
193.	NOR4_Y3 
194.	NOR4_Y4 
195.	NOR4_Y6 
196.	NOR4_Y8 
197.	NOR4_Y10 
198.	NOR4_Y20 
199.	NOR4_Y40 
200.	NOR4_Y80 
201.	NOR4_Z1 
202.	NOR4_Z2 
203.	NOR4_Z3 
204.	NOR4_Z4 
205.	NOR4_Z6 
206.	NOR4_Z8 
207.	NOR4_Z10 
208.	NOR4_Z20 
209.	NOR4_Z40 
210.	NOR4_Z80 
211.	DFF_X80 



**2. Find all the pins of the cell NAND2_X1 in simple_max.lib**


   	pin ("o")
  	pin ("a")
  	pin ("b")

![pinn0](https://user-images.githubusercontent.com/108817818/220407398-485e082e-bf7a-4ef4-952a-bd5b2186fd7a.jpg)

![pina b](https://user-images.githubusercontent.com/108817818/220407434-b98b8aca-8595-4cd2-a6dc-302d79a9584e.jpg)

**3. What difference you see between NAND2_X1 and NAND3_X1**


NAND2_X1 is a 2 input NAND Gate with pin 'o' , 'a' , 'b'
 NAND3_X1 is a 3 input NAND Gate with pin 'o' , 'a' , 'b' , 'c'
 
 Apart from that Max Capacitance of output pin "o" is different. 

   ![nand2ocap](https://user-images.githubusercontent.com/108817818/220414497-da5b5109-20c4-44b0-a376-2bc7e82d7ac3.jpg)
    ![nand3pino](https://user-images.githubusercontent.com/108817818/220414513-8e1dbfc4-f01a-404f-9081-b32aca81e29a.jpg)
		
![comparenand](https://user-images.githubusercontent.com/108817818/220416333-174d0d66-6092-430a-94d2-5c9a3b162134.jpg)

**4. What is the difference between ‘simple_max.lib’ and ‘simple_min.lib’**












**SPEF (Standard Parasitic Exchange Format)**

It describes parasitic information of the design and is automatically generated by the tool.It is mainly used to pass parasitic information from one tool to
another.
 
A Typical SPEF File has 4 main sections
• Header
• Name Map
• Top Level Ports
• Parasitic description


 Command for spef parsing

                  Cmnd: read_spef
									
									
									
![spef](https://user-images.githubusercontent.com/108817818/220420634-ecabe614-b2db-4d6a-b9ae-8a37461b91ae.jpg)

**TIMING REPORT EXERCISE**

Add Command in run.tcl file:-

            report_timing –num_paths 5
						
Rerun        

           sta run.tcl –exit | tee run.log					
					 
						
![runn](https://user-images.githubusercontent.com/108817818/220425067-d5dc2dda-1153-41bb-984d-a3fd5300441a.jpg)



![report1](https://user-images.githubusercontent.com/108817818/220424938-2b6cd36c-8023-4314-a4fe-9aa4f10f1d3a.jpg)



## **LAB 3**
**SLACK COMPUTATION**

Command to run OPEN STA and save software related information to text file name out.txt


                   sta run.tcl -noexit | tee out.txt
									 
									 

![running lab](https://user-images.githubusercontent.com/108817818/220434206-734678ac-1af7-4ece-8fc6-91084f769be1.jpg)


out.txt file:-
       
			                     leafpad out.txt


![out](https://user-images.githubusercontent.com/108817818/220437793-ff54361f-70ca-4551-8f55-d61b6dbfaaa8.jpg)



CIRCUIT TO PERFORM SLACK CALCULATION




![circuit](https://user-images.githubusercontent.com/108817818/220438554-4acc9dc2-40f9-4e2d-865d-60a817ab3ccc.jpg)

![path11222](https://user-images.githubusercontent.com/108817818/220442536-7c98ef80-680a-4765-8b23-b7e0ff381ab1.jpg)

**Change the number of Paths**


![run tcl](https://user-images.githubusercontent.com/108817818/220443283-8f66c0e1-18a4-47b6-a237-6de5523f1e64.jpg)


PATH 1

![path111](https://user-images.githubusercontent.com/108817818/220455720-ea6a2260-8930-4231-8599-28e919717a53.jpg)



PATH 2


![path22](https://user-images.githubusercontent.com/108817818/220449967-2c7105b1-b11e-418c-aebf-3f73c9eb8ba0.jpg)



PATH 3


![path33](https://user-images.githubusercontent.com/108817818/220451087-122ea7e2-fcbb-44e5-9605-a380bc22ead4.jpg)


PATH 4

![path4](https://user-images.githubusercontent.com/108817818/220455220-2ab057ce-6ab2-49b1-82f1-cbe448cae121.jpg)



PATH 5

![path 5](https://user-images.githubusercontent.com/108817818/220455244-a27b55d3-a815-4cdf-8e02-0e25470daf33.jpg)


PATH 6
![path 6](https://user-images.githubusercontent.com/108817818/220455270-a3911aa5-784d-4f79-a22a-309fdec45274.jpg)


PATH 7
![path 7](https://user-images.githubusercontent.com/108817818/220455301-949a0db8-43d1-4c7a-a16c-515df871bd48.jpg)


PATH 8![path 8](https://user-images.githubusercontent.com/108817818/220455340-0c2beeae-4aa4-44bd-8b87-cf62d12ff234.jpg)


## **LAB 4**

**1. Clock Gating Check**


 Gating techniques used is **‘Active Low Clock Gating’**
 
 		cd lab6
		leafpad run.tcl
															     
	
![run tcl](https://user-images.githubusercontent.com/108817818/220466136-bf952aac-46a6-4c07-9f4f-221df737521d.jpg)


                            sta run.tcl –exit | tee run.log


**SLACK ON CLOCK GATING PATH REPORTED**


![staarunnnfirst](https://user-images.githubusercontent.com/108817818/220466455-64944079-b64d-4b25-8ea9-0e92f71b80f8.jpg)
![starun2](https://user-images.githubusercontent.com/108817818/220466695-00c097d2-2df1-4bfc-853f-66c4a95b41bd.jpg)


**2. Async Pin Checks**			
           	 
								 
								 
	cd lab7					 
	leafpad run.tcl
																				
![run tcl](https://user-images.githubusercontent.com/108817818/220466888-be3e265b-8a9c-424a-9de8-970606f1cb14.jpg)
		
						
		
	      sta run.tcl –exit | tee run.log
																	
																					 
																	 
![run1111111](https://user-images.githubusercontent.com/108817818/220467204-183ceb3d-2cd8-4e78-b38c-c18d706c19cf.jpg)



## **LAB 5**

Common Path Pessimism Removal(CPPR)
Common path pessimism removal (CPPR) is the removal of artificially-induced pessimism between a launch and capture flip-flop pair during timing analysis by identifying the common clock path between launch and capture clock paths.
			
			
![photu crpr](https://user-images.githubusercontent.com/108817818/220470494-2e638a5b-dca0-4ea1-b468-4c843ec0e08b.jpg)

**TIMING REPORT BEFORE CPPR**

 
 
     cd lab4
	  sta run.tcl –exit | out.txt


![run tcl0](https://user-images.githubusercontent.com/108817818/220471545-16c42e8d-6d1d-4a5c-94bd-062b2671915a.jpg)


	 
![1st report](https://user-images.githubusercontent.com/108817818/220471574-8a237c75-9242-4e03-859b-9e381935467b.jpg)


							 
**TIMING REPORT AFTER CPPR**

‘c2’ is node which requires CPPR

Now change (following from 0 to 1)


       set sta_crpr_enabled 1
	

![run tcl1](https://user-images.githubusercontent.com/108817818/220471607-275bddba-c778-40bd-a280-7a3a89e5056d.jpg)
![updated report](https://user-images.githubusercontent.com/108817818/220471627-272b5573-3c68-4b89-9957-3ae82470adb3.jpg)

ON COMPARING

![COMPARIMG REPORT](https://user-images.githubusercontent.com/108817818/220473378-a2ca1b34-98c9-4c53-8c5a-f2e25ab3ad68.jpg)

**ECO – Engineering Change Order**





																				 
																				 
															 


