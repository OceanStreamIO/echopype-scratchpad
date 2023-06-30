# Q&A


**Q: What is the difference between single and multibeam echosounders in terms of the number of frequencies used?**

A: Single beam echosounders typically operate at one or two frequencies to measure depth and sometimes to provide some information about bottom characteristics. On the other hand, multibeam echosounders usually operate at a wide range of frequencies. The specific frequency used can vary depending on the water depth, with higher frequencies used for shallow waters and lower frequencies for deeper waters. Multibeam echosounders may also utilize frequency-modulated (chirp) signals to increase the signal-to-noise ratio and provide better resolution.

**Q: What does the number of beams refer to in an echosounder system?**

A: The number of beams in an echosounder system refers to how many separate directions of sound pulses, or beams, the system transmits and receives. A single-beam echosounder sends out a single sound pulse straight down and listens for its echo. A multibeam echosounder sends out multiple sound pulses at different angles to create a 'swath' of sound that covers a larger area of the seafloor or water column. The specific configuration, single-beam or multibeam, depends on the design of the system and the requirements of the application.

**Q: How do single and multibeam echosounders differ in terms of angle of arrival computation?**

A: In a single beam echosounder, the angle of arrival plays less of a role, as the sound pulse is sent directly down and the depth is measured based on the time it takes for the pulse to return. Some advanced single beam systems (like split-beam or dual-beam echosounders) can provide limited directional information about the source of the returning sound pulse by splitting the outgoing sound pulse and the returning echo into separate beams and measuring the phase difference or time delay between these beams.

In contrast, the angle of arrival is important in multibeam echosounders. Each beam in a multibeam system has a different angle, and the system uses phase detection methods to calculate the angle of arrival of the echo. This angle is then used to compute the depth and position of the seafloor. Multibeam echosounders require advanced signal processing and computing power to handle the data from all the different beams and frequencies, allowing them to provide a more detailed and accurate representation of the seafloor.

**Q: What does it mean if an echosounder's netCDF file only includes the "backscatter_r" component and not the "backscatter_i" component?**

A: If an echosounder's netCDF file only includes the "backscatter_r" (real) component and not the "backscatter_i" (imaginary) component, it typically means that the system is only providing the amplitude information of the backscattered signal, and not the phase information. In such systems, the "backscatter_r" represents the strength or intensity of the backscattered signal, which can provide useful information about the characteristics of the seafloor or other objects in the water column.

**Q: What do the terms Broadband (BB) and Continuous Wave (CW) refer to in the context of an echosounder system?**

A: The terms Broadband (BB) and Continuous Wave (CW) refer to the frequency characteristics of the sound pulses that an echosounder system transmits. A CW system transmits a sound pulse at a single constant frequency, while a BB system transmits a frequency-modulated sound pulse that covers a range of frequencies. This frequency modulation in BB systems can help provide higher resolution data and improved signal-to-noise ratio compared to CW systems.

**Q: What is the difference between Broadband (BB) and Continuous Wave (CW) modes in echosounder systems?**

- A Continuous Wave (CW) system transmits a signal at a constant frequency.
- A Broadband (BB) system transmits a frequency-modulated "chirp" that covers a range of frequencies. This chirp usually starts at a lower frequency and increases to a higher frequency, covering a band of frequencies in the process. The use of a range of frequencies and frequency modulation helps BB systems to provide higher resolution data and improved signal-to-noise ratio compared to CW systems. This could mean better ability to distinguish different types of seafloor, detect and identify objects in the water column, or map the seafloor in detail
