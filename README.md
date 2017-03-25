# VbD-Study
This repository contians materials of a study comparing people’s visualization construction and data exploration process using two visualization tools: one implementing the manual view specification technique (Polestar) and another implementing the visualization by demonstration technique (VisExamplar).

# Repository's Map
There are four main folders in this repository: Analysis, Datasets, Raw Data, Task + Demographic forms

** ***Analysis:*** 
This folder contains the results of our data analysis using in both SPV and pdf formats.

** ***Datasets:*** 
This folder contains the two Cars and Movies datasets used in our experiment.

** ***Raw Data:*** 
This contains the raw data collected from the experiment. 

** ***Tasks + Demographic forms:*** 
This folder contains the list of tasks used in Phase 1 of our study and demographic questions participants asked to answer.

# Two Visualization tools used in our study

The main experiment of this study entailed the use of two visualization tools, <a href="https://github.com/BahadorSaket/VbD">VisExamplar</a> and <a href="https://github.com/vega/polestar">Polestar</a>, which satisfied two requirements. One is that each had to clearly embody one of the two interaction techniques examined in this paper. The other is that to have a fair comparison between these two techniques, users had to be able to learn and use the system within the duration of the experiment. As each tool adopted only one of the two interaction techniques, we compared VisExamplar, which incorporates visualization by demonstration and Polestar, which incorporates manual view specification. We previously developed VisExamplar to show the feasibility of the visualization by demonstration paradigm. For this study we extended the previous implementation by adding some additional features and improving some of the underlying algorithms. Although a variety of commercial tools incorporate the manual view specification technique, we decided to use the less complicated visualization tool, Polestar, to control for external factors that might affect the study. Also, Polestar has previously been used in other studies to contrast recommendation browsing technique with manual view specification.


<strong><a href="https://github.com/vega/polestar">Polestar:</a></strong> (shown in Figure  below) is a visualization toolthat implements the manual view specification  paradigm.   Polestaris Tableau-style user interface for visual analysis, building on top of Vega-Lite. Polestar user interface consist of a Left-side panel, Encoding Shelves, and the Main View. The Left-side panel presents thedata schema, listing all data attributes in the dataset. Encoding Shelveslocated next to the data schema and represent different encoding channels. Users can drag and drop a data attribute onto a shelf to establisha visual encoding. They can also change properties of the data (e.g.,data types, data transformations) or the visual encoding variable (e.g.,color or sort) via pop-up menus. Main View of the Polestar shows acreated visual representation. Upon user interaction, Polestar updatesthe visual representation shown on the main view.

![polestar](https://cloud.githubusercontent.com/assets/4343770/24326749/cfbf6ad0-118b-11e7-8d13-9c40c51edbe4.png) 

<strong><a href="https://github.com/BahadorSaket/VbD">VisExamplar:</a></strong> VisExamplar tool (shown in Figure below) consists of two main components: demonstrations provided by users to show their intended actions and transformations that are recommended by the system in response to the given demonstrations. To provide demonstrations, VisExamplar supports two methods. One is that it allows users to directly adjust the spatial layouts of data points (e.g., users stacking data points in the shape of bars to convey their interest in a barchart) and the other, which allows users to provide demonstrations by adjusting the graphical encodings used in a visualization (e.g., users changing the size of data points in a scatterplot). In response to the provided demonstrations, VisExamplar recommends four categories of transformations (change the current visualization technique, define mappings between graphical encodings and data attributes, assign data attributes to axes of a visualization technique, change the view specifications without changing the underlying technique). By accepting any of the recommended transformation the system will change the corresponding view.

The VisExemplar user interface consists of a ThinkBoard, Recommendation Gallery, and a Detail View panel. Users can construct their demonstrations through direct manipulation of the visual representation on the ThinkBoard. Some of the recommendations (e.g., recommending data attributes to be mapped to axes) might also be shown on the ThinkBoard. Other recommendations will be presented in the Recommendation Gallery. The primary goal of the Detail View panel is to show data attribute types and values for a selected data point. For more details about the VisExamplar please refer to main work which describes this system.

![capture](https://cloud.githubusercontent.com/assets/4343770/24326793/1181e9e2-118d-11e7-8e06-adfa7d4d47e8.png)
