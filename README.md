# MathematicaWebScrape
*Both the Mathematica notebook and plain text version are provided* 

*Description of AutoScrape Function:*

-Input is a list of text you desire to input to MesHonDemand website.

-Function loops from 1 to N (N being length of list of text. For my case N = 17 because there are 17 indicators.

-StartWebSession Documentation: https://reference.wolfram.com/language/ref/StartWebSession.html

-WebExecute Documentation: https://reference.wolfram.com/language/ref/WebExecute.html

-Calls of the WebExecute function saved as variables are pointers to positions of interest on website. Those variables are proceeded by calls of the WebExecute function that interact with the desired element in a specific way denoted by the first phrase in quotes. All WebExecute uses are noted in the Documentation. 

-All "Pause[]" in the code are used to allow for the website to load.

-Once text is exported, it is parsed and only the desired Mesh terms remain. If you want to keep the rest of the data it is found in the "PageText" variable.

-Since there are a varying amount of Mesh terms per SDG, the Mesh term lists are padded with empty spaces to ensure a square matrix that can be transposed for optimal excel exporting.
