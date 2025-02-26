# Setup and Use

## Installation 
There are two main components to install. The PC based Workbench and the mainframe based Performance Engine.

- To build and install the Workbench go to [GenevaERS Workbench github.](https://github.com/genevaers/Workbench)

- To download the latest Performance Engine executables go to [GenevaERS Performance Engine releases in github.](https://github.com/genevaers/Performance-Engine/releases)

- For information on how to use the Workbench to create a new view, follow the examples under [Basic Skills.](#basic-skills) 
  
- To run a view look at the sample JCL in [Running the View.](RunView/RunView.md)

- For more advanced knowledge look at [Advanced Features.](../AdvancedFeatures/index.md)  
  
- For tuning and parameter reference information go to the [Reference.](../Reference/index.md)

## Basic Skills

The examples here are based on the Demo data. If you haven't installed the Demo, then it is highly recommended you do. [Find the Demo here.](https://genevaers.github.io/Demo/)

The following Workbench tasks are based on the Workbench user having **system administrator** rights. For more information on users and access rights go to [Workbench security overview.](../AdvancedFeatures/SecurityOverview.md)

**Import the Demo XML into the Workbench in a new environment**

1. Download the Workbench XML [DemoOpen.xml](https://github.com/genevaers/Demo/blob/main/XML/DemoOpen.xml) from the Demo repository, to a folder on your PC.  
(Alternatively, using your preferred file transfer method, download the data set created during the Demo installation, *your-hlq*.GVBDEMO.WB.XML, to a folder on your PC.)
2. Start up the Workbench.
3. Select **Administration** > **New** > **Environment**
4. In the **Name** field type **DemoEnv**
5. Uncheck **Generate a Control Record**
6. Save the environment definition **File** > **Save**
7. Select **Administration** > **Import**
8. Type the following in the Import Utility window
    - Target Environment: **DemoEnv**
    - Component Type: **View Folder**
    - Archive Folder: ***your-PC-folder***
9. Select the XML file that is listed in **File(s)**
10. Click **Import**

This imports in to the Workbench all the PFs, LFs, LRs, Lookup Paths, and Views associated with the Demo.
 
You can now create a new view using some of the Demo metadata.

[Example 1: Creating a new view](Examples/NewView.md)

[Example 2: Adding a filter](Examples/AddExtractFilter.md)

[Example 3: Adding a lookup field](Examples/AddLookup.md)

[Example 4: Adding column logic](Examples/AddColumnLogic.md)

[Example 5: Creating a summary view](Examples/NewSummaryView.md)


