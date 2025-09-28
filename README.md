![STK Logo](/assets/stk.svg)

# STK Master Certification

<a href="https://help.agi.com/stk/Content/training/TutorialOverview.htm" style="display: inline-block; background-color: #5b17f8ff; color: white; padding: 10px 20px; text-align: center; text-decoration: none; border-radius: 5px; font-weight: bold;">STK Training Tutorials</a>


## EXERCISE 1
### Model aircraft missions with Aviator

![Ex1 Banner](/assets/banner.png)

**Which of the following answers is correct concerning enabling Delay Enroute Climbs and Descents in Aviator?**

- **The aircraft begins climbing or descending at a point in time during the procedure such that it won't achieve the new altitude until the start of the arc or pattern, or until it has reached the procedure site.**

**What is the length of runway 01R / 19L at Andrews AFB?**  
- **9755 feet**
  
**The mission aircraft is overhead PUB at approximately 19:52:00. At that time, what is its approximate ground speed?**
- **480 nm/hr**

**Approximately how much fuel was consumed during the mission?**  
- **43,067 lb**

**Approximately, how long does the flight take from takeoff at Andrews AFB to landing at Edwards AFB and coming to a complete stop?**  
- **4 hours 19 minutes**

---

### Data extracted from Report `ex1/MissionAcft_Ex1_3_4`

| Date and Time            | Ground Speed (nm/hr) | Fuel Consumed (lb) |
|--------------------------|----------------------|---------------------|
| 1 May 2024 19:52:14.064  | 479.621642           | 28,591.107          |
| ...                      | ...                  | ...                 |
| 1 May 2024 21:19:03.673  | 7.160344             | 43,066.861          |


---

![Ex1.2 Banner](/assets/radar.png.bmp)

**Basing a probability of detection on an S/T Integrated PDet value of 0.8 or higher, approximately what time can you be certain of first tracking the aircraft?**
- **19:43:00**

**When the aircraft is outbound from PUB, what is the approximate distance from the radar to the aircraft when the S/T Integrated PDet value drops below 0.8?**
- **141 km**

**What is the approximate S/T Integrated Signal to Noise Ratio (SNR) when an S/T Pulses Integrated value of 1 is first achieved?**
- **16 dB** 

**Basing a probability of detection on an S/T Integrated PDet value of 0.8 or higher and not considering the time the aircraft is in the radar’s cone of silence, what is the approximate length of time the radar can track the aircraft? Round times up or down as needed.**
- **17 min**

**Basing a probability of detection on an S/T Integrated PDet value of 0.8 or higher, what is the approximate elevation angle of the aircraft from the radar site the first time 0.8 is achieved?**
- **3.6 deg**

---

### Data extracted from Report `ex1/Place-PUB-Sensor-Servo-Radar-Radar-To-Aircraft-MissionAcft_Radar_SearchTrack`

---

## EXERCISE 2
### Model satellital missions with Astrogator


![Ex2 Banner](/assets/astrogator_frame.png.bmp)

**What was the approximate Delta-V Magnitude used to raise the Apoapsis to 22000 km?**
- **2.0 km/sec**
  
**What is the approximate amount of estimated fuel used for the maneuver?**
- **496 kg**

**What is the approximate estimated burn duration for the maneuver?**
- **2917 sec**

**What is the purpose of setting the Action to Run active profiles?**
- **It runs the mission control sequence allowing the active profiles to operate.**

**How does Astrogator calculate an impulsive maneuver?**
- **It calculates the new state of the spacecraft by adding a Delta-V vector to the final state 
velocity of the previous segment.**

---

### Data extracted from Report `ex2/CommSat_Segment_Summary`

| **Maneuver Summary**                                 |                                                              |
|------------------------------------------------------|--------------------------------------------------------------|
| **DeltaV Magnitude**                                 | 2014.215637782269 m/sec                                       |
| **Estimated Equivalent Finite Burn Duration**        | 2916.868406451747 sec                                         |
| **Estimated Fuel Used**                              | 495.73 kg                                                     |
| **Maneuver Direction Specification**                 | Along Velocity Vector                                         |

---

![Ex2 link](/assets/link.png.bmp)

**Do you have any BER values greater than 1.000000e-009?**
- **No**

**Do you have any BER values greater than 1.000000e-009? (After update G/T to 17 dB/K)**
- **Yes**

**When the first instance that your BER is greater than 1.000000e-009, what is the approximate range from the Place object to the Satellite object?**
- **25270 km**
  
**When the Transmitter object has Access to the Receiver object, approximately, what is the closest range between the two objects?**
- **1089 km**

**What is the approximate Elevation angle between the Transmitter object and the Receiver object when the BER in the Link Budget - Detailed report is highest?**
- **0.6 deg**

---

### Data extracted from Report `ex2/Place-Raisting-Receiver-DLRx-To-Satellite-CommSat-Transmitter-DLTx_Link_Budget_-_Detailed` and `ex2/Place-Raisting-Receiver-DLRx-To-Satellite-CommSat-Transmitter-DLTx_AER` 



* First instance that BER is greater than 1.000000e-009 (@ 1 May 2024 10:47:30.000).


| **Time (UTCG)**               | **Azimuth (deg)** | **Elevation (deg)** | **Range (km)**     |
|-------------------------------|-------------------|---------------------|--------------------|
| 1 May 2024 10:47:48.000       | 222.092           | 22.832              | 25270.404653       |


* Closest range between Receiver and Transmitter.

| **Event**        | **Time (UTCG)**           | **Azimuth (deg)** | **Elevation (deg)** | **Range (km)**     |
|------------------|---------------------------|-------------------|---------------------|--------------------|
| Min Elevation    | 1 May 2024 06:27:40.066   | 297.985           | 1.185               | 2770.156568       |
| Max Elevation    | 1 May 2024 06:33:48.237   | 227.546           | 30.905              | 1088.827302       |
| Mean Elevation   | -                         | -                 | 13.991              | -                  |
| Min Range        | 1 May 2024 06:33:48.889   | 227.255           | 30.905              | 1088.817868       |
| Max Range        | 1 May 2024 06:27:40.066   | 297.985           | 1.185               | 2770.156568       |
| Mean Range       | -                         | -                 | -                   | 1876.291015       |

* Elevation angle when BER is highest (@ 2 May 2024 09:19:42.263).

| **Time (UTCG)**               | **Azimuth (deg)** | **Elevation (deg)** | **Range (km)**     |
|-------------------------------|-------------------|---------------------|--------------------|
| 2 May 2024 09:19:42.263       | 333.790           | 0.595               | 27816.691113       |

---