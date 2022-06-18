# Problem Statement-
(Vectech)(https://www.vectech.io/) is a technology social enterprise working to empower public health organizations in the global fight against mosquito-borne disease, which wants to develop a species identification model for mosquitoes. For better identification, they wanted help in developing a mosquito body part segmentation and identification model  to help us determine what parts of the mosquito are visible and intact in the image. This enables more advanced computer vision methods, serving as highly valuable prior information for the species identification CNN, and may be paired with entomological taxonomic information to improve identification accuracy. These advanced methods are required for mosquito surveillance products because captured mosquitoes from the wild are often very damaged, missing scales, wings, legs, etc., which  sometimes affects whether that mosquito can be accurately identified to its species.
 
 The main objective of the project is to identify the specific portions of the image that are the legs, abdomen, wings, and other important body parts of the mosquito 
given a standardised image of a mosquito. The parts have to be identified and labelled with their names. The AI solution should work with similarly standardised images
as those produced by our devices. The best solutions will have high resolution segmentation that includes very small features like the hairs on mosquito legs andabdomen.
These features are critical for identification and their presence, absence, and number can enable assessment of the physical condition and whether a specimen can be 
identified to species using the output segmentation.

# Pipelines I worked in:-
  ### 1) **Data Annotation**
        -    Annotated 500+ images
        -    Worked as supervisor (reviewed 3000+ annocationn)
        -    Managed annotation team and helped in co-ordinating between collaborators of the different time zone to ensure smooth progress
        -    Tools Used - CVAT and Scale Rapid
  ### 2) **Modelling**
        -    #### **Build multiple models using tensorflow framewore:-**
        -    
