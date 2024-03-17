---
layout: post
title:  "Supercritical Carbon Dioxide (sCO2) in HVACR/Hot Water"
subtitle:  "If you wanna drive, learn to throw a wrench first!"
date:   2024-03-12 4:30:00
categories: template
---


# Module 1: Fundamentals of Supercritical CO2

* Carbon Dioxide (CO2) exhibits distinct properties depending on its state (solid, liquid, gas) that make it an attractive option for heat pumps, particularly in the higher temperature, higher pressure supercritical state (sCO2)

    * Solid (Dry Ice): At very low temperatures (-78°C), CO2 becomes a solid (dry ice). It has a low density and poor heat transfer capability.
    * Liquid: Under normal pressure and above -78°C, CO2 exists as a liquid. It has a higher density than solid CO2 and a moderate heat capacity (ability to store thermal energy). However, its ability to absorb and release heat through phase changes (boiling/condensing) is limited compared to other refrigerants.
    * Gas: Above its critical temperature (31°C) and critical pressure (7.3 MPa), CO2 enters the supercritical state (sCO2), which KEY as state enabling heat pump, refrigeration and hot water applications.

* Supercritical CO2 (sCO2) is where things get interesting/advantageous for heat pump systems:
    * sCO2 maintains a relatively high density like a liquid, but behaves like a gas with high diffusivity (ability to spread and mix). This allows for compact heat exchangers compared to traditional vapor-compression cycles.
    * By adjusting pressure slightly above the critical point, the density and heat capacity of sCO2 can be continuously varied. This allows for fine-tuning the heat transfer process across a wider temperature range.
    * CO2 exhibits good thermal conductivity (ability to conduct heat) in the supercritical state. This translates to efficient heat absorption from a low-temperature source (ground, air) and heat release at a higher temperature for heating purposes.
    * The ability to operate effectively across a wider temperature range and efficient heat transfer contribute to a higher Coefficient of Performance (COP), meaning more heat output for less energy input and smaller heat exchangers due to the high density of sCO2 allow for more compact heat pump units.
    * CO2 is a naturally occurring and non-toxic, thus a safer, more environmentally-friendly refrigerant which [especially consideering all of the other benefits in performance and efficiency] an extremely low global warming potential (GWP) compared to traditional refrigerants.
    * sCO2 systems do have higher operating pressures, thus require higher quality, but standard fittings with thorough validation of assemblies which will ensure the system safely withstands high pressures.
    * The use of sCO2 presents [corrosion engineering, material selection and design issues](https://energy.sandia.gov/wp-content/gallery/uploads/SAND-2014-0602C.pdf), which are certainly not insurmountable by any means, but they must be addressed. Specifically, materials in power generation components must display high-resistance to damage caused by high-temperature, oxidation and creep. Candidate materials that meet these property and performance goals include incumbent alloys in power generation, such as nickel-based superalloys for turbomachinery components and austenitic stainless steels for piping. Subcritical [Brayton cycle loops](https://en.wikipedia.org/wiki/Brayton_cycle) which have gas as their working fluid suffer from even minute traces of water vapor contamination [seen even in closed, de-watered systems] and, as such, [carbonic acid](https://en.wikipedia.org/wiki/Carbonic_acid) formation causes corrosion and erosion, specifically erosion in turbomachinery and recuperative heat exchanger components and intergranular corrosion and pitting in the piping.
    * If the system design is not **open source technology**, then sCO2 HVACR systems could really increase initial costs. However, this is an area for open source to make a huge difference, these fittings are relatively simple to manufuacture and could be manufactured in volume as COTS standard hardware. The pressure validation process is straightforward but it must be done correctly by someone with professional-level skills who understands key concepts of high pressure sub-assembly and assembly validation, but validationg sCO2 HVACR construction is safer than chemically-based refrigerant HVACE systems sincy there's no chance of escape of toxic liquids/gases or any disagreeable odors.
    * Precise internetworked control and monitoring systems would be advisable [but not required] for maintaining optimal pressure and temperature conditions and off-site reporting of continuously monitored data for efficient and assuredly safe operation.

* There are several thermodynamic cycles that can be utilized with supercritical CO2 (sCO2) for various applications, including heat pumps. two more prominent cycles are the **transcritical cycle** and the **subcritical cycle**.  The transcritical cycle is the most common cycle used in sCO2 heat pumps.  The subcritical cycle operates similarly to the transcritical cycle, but with a key difference: CO2 reaches a supercritical state only during compression. After heat rejection, it enters a two-phase region (partially liquid, partially gas) before entering the expander.  The selection between transcritical and subcritical cycles depends on various factors, including temperature requirements, system complexity, and efficiency.  Both cycles can achieve high efficiencies, but the transcritical cycle may offer a slight advantage due to simpler operation in the supercritical state throughout.

    The **TRANScritical** cycle is the most common cycle used in sCO2 heat pumps. [For heating use] the CO2 vapor is compressed in a compressor [probably outdoor, or not in the house, but immediately downstream of the external heat exchanger], increasing its pressure and temperature. The hot, high-pressure sCO2 then flows through [insulated lines of] the system to enter the internal heat exchanger, transferring heat to the heating system (internal water loop) at a temperature above the sCO2 critical point, ie, the sCO2 remains in a single phase (supercritical) despite the temperature change. In the next stage, the CO2 then undergoes expansion in a turbine or expander, converting some of the pressure energy back into mechanical work to help drive the compressor and reducing its temperature. The cooler, low-pressure but still supercritical sCO2 then flows through the external heat exchanger, absorbing heat from the low-temperature source (ground, air). Due to the unique properties of sCO2, even small pressure TRANS-state changes, with sCO2 always staying within the boundaries the supercritical state, significantly affect its ability to absorb heat. After giving off heat to the heat-exchanger, the cycled sCO2 re-enters the compressor, and the **TRANScritical** cycle repeats. This cycle is, of course, reverse for the cooling uses.

    The **SUBcritical** cycle operates similarly to the transcritical cycle, but with a key difference being that CO2 reaches a supercritical state ONLY during compression; after heat rejection, it enters a two-phase region (partially liquid CO2, partially gas C02; not [supercritical fluid C02](https://en.wikipedia.org/wiki/Supercritical_fluid) before entering the expander. An additional heat exchanger (desuperheater) might be needed before the expansion process to remove excess heat and ensure the CO2 enters the expander ***entirely*** as a liquid for efficient work extraction.

**Choosing the Right Cycle:**

The selection between transcritical and subcritical cycles depends on various factors, including:

* **Temperature Requirements:** Transcritical cycles are better suited for applications where the heating demand requires higher discharge temperatures.
* **System Complexity:** Subcritical cycles might require additional components like a desuperheater, increasing complexity.
* **Efficiency:** Both cycles can achieve high efficiencies, but the transcritical cycle may offer a slight advantage due to simpler operation in the supercritical state throughout.

**Additional Notes:**

* These are simplified explanations, and real-world sCO2 cycles might incorporate additional components like intercoolers for further efficiency improvements.
* Research is ongoing to optimize sCO2 cycles for various applications, including waste heat recovery and integration with renewable energy sources.

* Advantages of sCO2 over traditional refrigerants 

**Module 2: sCO2 Components and System Design**

* Compressors, expanders, and heat exchangers for sCO2
* System configurations: Transcritical, subcritical, cascade
* Piping, materials, and safety considerations

**Module 3: sCO2 in Refrigeration Systems**

* Applications in commercial and residential refrigeration
* Design optimization for sCO2-based systems
* Performance and energy efficiency analysis

**Module 4: sCO2 in Air Conditioning**

* Applications in space cooling and dehumidification
* Integration with air-handling units and ventilation systems
* Control strategies for sCO2 air conditioning 

**Module 5: sCO2  Water Heaters**

*  Heat pump water heater principles with sCO2
* System configurations and designs
* Performance metrics and efficiency comparisons 

**Module 6: Combined HVACR Systems using sCO2**

* Integrating refrigeration, air conditioning, and water heating with sCO2 
* Energy optimization and waste heat recovery

**Module 7: Control Systems for sCO2 Applications**

* Sensors, actuators, and control algorithms for sCO2 systems
* Strategies for maintaining optimal performance and safety

**Module 8:  Installation and Maintenance**

* Best practices for installing sCO2 systems
* Leak detection and mitigation
* Troubleshooting and maintenance procedures

**Module 9:  Regulations and Standards**

* International and regional standards for sCO2 systems
* Safety considerations and environmental impact

**Module 10:  Market Trends and Future of sCO2**

*  Market growth and adoption of sCO2 in HVACR
* Research directions and technological advancements 
* Cost analysis and economic viability 
 
Let me know if you'd like more detail on any of these modules! 
