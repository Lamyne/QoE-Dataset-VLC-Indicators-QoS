# QoE-Dataset-V2-VLC-Indicators-QoS-parameters

This work is proposed to describe and to share a new subjective QoE dataset that assess YouTube video quality in controlled
laboratory environment. This dataset is an improvment for our published dataset (https://github.com/Lamyne/QoE-Dataset-VLC-Indicators/) that concerns QoE assessment using VLC player indicators. In fact, it is collected using the subjective Absolute Category Rate (ACR) method based on Mean Opinion Score (MOS) ratting score. The used platform is composed by the following components:
• VideoLAN  Client  player  (VLC):  To  display  YouTube video with its URLs (Uniform Resource Locator).
• Netem (Network Emulator): To generate the QoS parameters variations (link bandwidth, packet loss rate, ...etc.).
• Python  language:  To  implement  GUI  (Graphical  User Interface).
• MySQL database server: To store all the desired QoE IFs values on the database.
• Several PVSs (Processed Video Sequences) are considered.
• Validation questions to check participants feedback and to clean the resulted datset.


Comparing to the first dataset, our impovements consist on collecting network parameters (QoS), in addition to the VLC indicators, by  using ”iperf” tool between  a server  and  the  used  device  to  test. In addition, we gather more device  characteristics by using  Python  and  linux command to have device’s information like: screen size, used ram, used memory, etc.



The testbed is achieved in the LiSSi laboratory (http://lab.lissi.fr/) around Paris city in France. 41 testers participated in the test campaign. All of them were researchers and students from different disciplines aged 20 to 37 years with few or no experience with video assessment experimentation. The collected QoE IFs concerns  VLC indicators or video parameters (QoA), network parameters (QoS), device chacteristics (QoD) and user's information (QoU) that VLC video player provides as indicator.





1- Source:

Creators: 
- Lamine Amour (lamine.amour@u-pec.fr) 
- Sami Souihi (sami.souihi@u-pec.fr) 
- Abdelhamid Mellouk (mellouk@u-pec.fr)

2- Data Set Information:

The dataset was built from a controlled laboratory testbed where 300 sample covering 29 Quality of Experience Impact Factors (QoE IFs). 
The used videos are of different types/complexities.

The geographical location of the testbed was the LiSSi laboratory (http://lab.lissi.fr/) around Paris city in France. 62 testers 
prticipated in the test campaign. All of them were researchers and students from different disciplines aged 20 to 37 years with
few or no experience with video assessment experimentation.

3- Attribute Information:

The dataset is presented in different formats/files as follows:

    CSV (Microsoft)
    ARF (Weka tool)
    data (Genral format)

Both files contain 29 QoE IFs and the Mean Opinion Scors (MOS)given by userss. 

 -- The attributes are (dontated by Lamine Amour, 
	lamine.amour@u-pec )
 	1)  id
	2)  QoS_bandwidth
	3)  QoS_packet-loss
	4)  QoS_delay
	5)  QoS_jitter
	6)  V_id-video
	7)  V_content
	8)  V_norm-bitrate
	9)  V_complexity
	10) V_complexity-class
	11) QoA_VLCresolution
 	12) QoA_VLCbitrate
	13) QoA_VLCframerate  
 	14) QoA_VLCdropped
	15) QoA_VLCaudiorate
 	16) QoA_VLCaudioloss
 	17) QoD-cpu_mhz-moy
	18) QoD-cpu_mhz-avg 
	19) QoD_cpu-nbr
	20) QoD-cpu_core-nbr
 	21) QoD_stepping
	22) QoD-cpu_bigo-mips
	23) QoD_carte-class
	24) QoD_screen-resolotion
	25) QoD_screen-dimension
	26) QoD_screen-mhz
	27) QoD-screen_blug-type
	28) QoD-ram_clock-speed
	29) QoD_ram-size
     30) MOS
	
	-- Each variable belongs to a category of QoE Influence Factors (QoE IFs) that consists:
	      - Newtork parameters (QoS) (2 to 5)
		  - Video content analysis results (6 to 10)
	      - VLC player indicators (QoA) (11 to 16)
		  - Device characteristics  (QoD)(17 to 29)
          - User's 	MOS scoe(30)		  
             
5. Number of Instances : 

      	class 1 (MOS = 1): 29  
		class 2 (MOS = 2): 66
		class 3 (MOS = 3): 73
		class 4 (MOS = 4): 69
		class 5 (MOS = 5): 63

6. Number of Attributes 
	
	30

7. For Each Attribute:

	All attributes are digit except, video content type (V-content)  user gender (QoU_sex) and 
	device screen size (QoD_screen_size)
	
	No statistics available, but suggest to standardise
	variables for certain uses. 

	NOTES: 
      
	  - 		  
		  
	  
	  - 19st (MOS) Mean Opinion Scroe that a tester will give at the end of each video view.
		   5 -> Excellent
		   4 -> Good
		   3 -> Fair
		   2 -> Poor
		   1 -> Bad

4- Related publications

(a) Lamine Amour, Sami Souihi, Said Hoceini, Abdelhamid Mellouk: An Open Source Platform for Perceived Video Quality Evaluation.
Q2SWinet@MSWiM: pages 139-140. November 2015.

(b) Lamine Amour, Sami Souihi, Said Hoceini, Abdelhamid Mellouk: A Hierarchical Classification Model of QoE Influence Factors. 
WWIC 2015: pages 225-238, May 2015.

(c) Lamine Amour, Sami Souihi, Abdelhamid Mellouk: ACR-based Subjective QoE Datasets to Quantify YouTube Video Quality. 
QoMEX 2018: pages xxx-xxx, 2015 (Submitted).

5- Citation Request:

The following citation is requested if you use the dataset:

Lamine Amour, Sami Souihi, Abdelhamid Mellouk: ACR-based Subjective QoE Datasets to Quantify YouTube Video Quality.
QoMEX 2018: pages xxx-xxx, 2015 (Submitted).
