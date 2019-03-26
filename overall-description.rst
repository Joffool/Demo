Overall Description
========================


System Functionality Overview
-----------------------------
    This system implemented in the form of a web application includes concise instructions that appear in the interaction with users in the first place, which shall guide the users through uploading their valid original data files. After receiving and analyzing the files that meet the constraints of input, our system will present a corresponding chart or table reflecting the state of distribution from the original data in the file. All the indexes will be illustrated via visual presentation. For example, our User Interface will require users to upload a .txt file with certain format, then within 10 seconds one scatter plot will be shown along with display of data in the file.
    To be specific, in the first edition of our web application OMG, files of data recording differentially expressed genes and their quantities will be uploaded and analyzed, visualized information such as a scatter plot will be returned in result.

Input Type and Format Requirements
----------------------------------
    For the current edition of our system, only one type of files will be legal and valid type for the data analyzing function. All files to be uploaded must be of plain text file (.txt) and no other types will be accepted by the system. This is only temporarily requirements of this version of application and will be updated with new and loose ones.
    In each plain text to be uploaded, all data in it must be arranged in these formats:
        *	Data must be TAB-delimited with three columns lead by three headers.
        *	Headers must consist of indexes gene ID and two quantities of controlled sample and knockout sample, e.g. gene_id, ControlSample and KnockoutSample.
    One sample of a valid input is shown below:
    ===========  =================  =================
      gene_id      ControlSample      KnockOutSample
    ===========  =================  =================
     AT1G01010      1.198558083        2.036161827
     AT1G01020      13.75736234        13.370796
     AT1G01030      0.833779536        0.203616183
     AT1G01040      9.58846466         7.126566394
     AT1G01046      0                  0
     AT1G01050      23.81482799        21.10821094
     AT1G01060      0.625334652        1.221697096
     AT1G01070      1.719670292        0.950208853
     AT1G01080      28.34850421        25.24840665
     AT1G01090      58.26034505        42.96301455
     AT1G01100      1066.508249        1308.030358
     AT1G01110      2.709783491        1.425313279
    ===========  =================  =================


Output Content and Style
-----------------------
    Once finishes analyzing the original data of uploaded files, system will present a scatter plot reflecting the distribution state of all expressed genes of two states of sample, along with a table sorting all the data by the index of logFC. In the plot, the X-axis will represent ControlSample in log2 scale, and Y-axis will represent KnockoutSample in log2 scale.
    One rough preview of an outcome sample of scatter plot of differentially gene expression is shown below where the up-regulated genes are shown in red dots, and down-regulated genes are shown in blue:
    .. image:: /image/plot.png
