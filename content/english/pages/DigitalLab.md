---
title: "Digital Lab"
date: 2025-09-19
draft: false

# Features
pagefeatures:
  - title: "Simulation of Virtual Microorganisms"
    image: "/images/Icon_ComputerScreenPythonBio.png"
    content: "The Digital Lab is a simulation environment for virtual microorganisms developed by the **BiotechData.Academy** in cooperation with the [Institute of Applied Microbiology, RWTH Aachen](https://www.iamb.rwth-aachen.de/cms/iamb/Forschung/~bgeqfy/Industrielle-Systembiotechnologie/lidx/1/). Detailed models of microbial physiology, metabolism and genetics reproduce relevant data to understand the benefits of diverse analytics experiments and to plan biotechnological optimization."
    button:
      enable: true
      label: "Open Digital Lab Simulation Platform"
      link: "https://biotechdata-academy.streamlit.app/"

  - title: "Technical Background"
    image: "/images/Icon_BiolMathExamples.png"
    content: "Different components of the biological and technical variables are modeled in suitable frameworks. Gene expression activity is based on the sequence of the promoter sequence and a random forest, trained on a T7 promoter library, forecasts the product concentration. The metabolic network is captured using genome scale metabolic models that contain all growth relevant reactions. The activity of each reaction can be estimated using flux balance analysis, a process by which the growth rate is maximised, based on constraints like substrate uptake rate. The substrate uptake rate in turn depends on the enzyme activities which are modeled using the Michaelis-Menten equation. The calculated growth rate determines the dynamic growth behaviour, which is modeled with standard physics based empirical laws, like the logistic growth of the Verhulst equation. The models employ organism- and condition specific parameters, most of which are unknown. To simulate general physiological behaviour, these parameters are randomly, but reproducibly, sampled from a realistic range."
    button:
      enable: true
      label: "Original Journal Publication with Details"
      link: "https://doi.org/10.1128/jmbe.00113-22"

  - title: "Microbial Fermentation"
    image: "/images/Icon_ContinuousBatchCult.png"
    content: "Microbial cultivations are simulated for batch and continuous fermentation. During batch fermentation, substrate is depleted and biomass and products accumulate. In continuous fermentation, the medium is replaced such that the concentrations of biomass, substrates and products remain constant."
    button:
      enable: false
      label: "Open Digital Lab Simulation"
      link: "https://biotechdata-academy.streamlit.app/"

  - title: "Process Analytics Data"
    image: "/images/Icon_Analyt-MassLCLight.png"
    content: "Fermentations are documented with a range of analytical instruments. The analytics measures various properties like the turbidity using photospectrometers, pH value, substrate concentration or metabolites with HPLC. We collaborate with the vendors of analytic instruments to format the results of the simulations according to the specfications of commonly used analytic devices. This prepares users to efficiently handle the output of normal experiment runs."
    button:
      enable: false
      label: "Open Digital Lab Simulation"
      link: "https://biotechdata-academy.streamlit.app/"

# Explore our resources, tutorials, and tools to enhance your biotech data skills. We have designed a digital lab for simulating virtual microorganisms for biotechnology: [https://biotechdata-academy.streamlit.app/](https://biotechdata-academy.streamlit.app/)


---