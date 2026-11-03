README:
=======

"Point Me QA" enables the semi-automatic identification of landmarks in 3D and 4D medical images. These landmarks can be used as reference points for image registration, image registration validation, or motion quantification. The software can be operated by users with no prior experience, aiming to provide academic support for the advancement of research in the field of Image-Guided Radiation Therapy (IGRT).

=========================
How to run the program:
1. Extract the downloaded file.
2. Open the "PointMeQA" folder and double-click the executable file, also named "PointMeQA".
3. Follow the instructions on how to use the software and check the output files generated and saved in the same folder.

==============
How to use:
1. Enter the patient's name and the dimensionality of the images to be used.
2. Click the 'Browse' button to locate the main directory containing the patients' image and structure subdirectories.
3. Enter the full name of the directory containing the image selected as the reference image, as well as its modality (CT or CBCT).
4. Enter the full names of the segmentations of interest to be used, separated by commas. These segmentations will only be used to restrict the regions in which landmarks are identified. If this field is left blank, the algorithm will use the entire image for landmark extraction.
5. For 3D images, a second image may optionally be specified as the moving image. You may also indicate whether a transformation resulting from image registration exists between the two images. If so, enter its full name. The transformation file must be located in the patient's directory and must be in .tfm format. For 4D images, specify the respiratory phases of interest for landmark identification, separated by commas. Values must range from 0 to 90, in increments of 10.
6. Select the distance(s) of interest to be used as metrics for identifying corresponding landmarks between images.
7. Select the image regions in which landmarks should be identified: high-contrast regions only, or both high- and low-contrast regions.
8. Finally, select the checkboxes according to your requirements: extract the names of the segmentations accompanying the images to use them as regions of interest (ROI) constraints; generate an analysis report using the identified landmarks; set a maximum residual distance between corresponding landmarks, eliminating those that are too far apart and may represent false correspondences; generate landmark coordinate files for each image, compatible with the 3D Slicer software; perform dose analysis using the identified landmarks, provided that the images include dose distributions; and calculate the Mutual Information (MI) between the provided images.
9. Click the 'Start' button to run the algorithm. It is normal for the program to display a "Not Responding" message while processing. However, the results will be generated normally.
10. Once processing is complete, select whether you wish to manually choose which corresponding landmarks to retain (semi-automatic extraction mode).
11. Depending on the images used, processing may take anywhere from a few minutes to several hours. Once completed, all output files will be saved in the same directory as the executable file.
12. If you wish to process another case, close the executable and open it again.

=========================
This computer program was registered with the Brazilian National Institute of Industrial Property (INPI) under registration number BR512024000601-0.
For further information or assistance, please contact: amandamazer18@gmail.com

=========================
How to cite / reference:

MAZER, Amanda C. Development of an algorithm for image registration assessment in Image-Guided Radiation Therapy (IGRT). 2024. PhD Dissertation (Nuclear Technology) – Institute for Energy and Nuclear Research (IPEN-CNEN/SP), São Paulo, Brazil.
