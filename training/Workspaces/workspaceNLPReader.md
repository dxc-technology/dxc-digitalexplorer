# DXC Digital Explorer - Workspace advanced document reader

_Released Nov 2020_
<br>

DXC Digital Explorer workspaces allows you the option to analyse documents or website and load the matching content into your workspace.

The advanced document reader leverages the [Azure Cognitive NLP](https://azure.microsoft.com/en-gb/services/cognitive-services/text-analytics/) services to provide a deep scan of the associated document.

The NLP updated scans the document against 3 core services 

- Named entities
- Linked entities
- Key phrases

Named and linked entities are matches against a managed dictionary within the Azure service, while key phrases are calculated by the NLP engine itself (and can create some interesting results).


## Access controls
Access to the enhanced document reader is currently restricted to users with "Trend Reviewer" role.

## Read Documents

The enhanced document reader presents 2 options

![image](images/enhancedDocumentReader.png)<br>

- Standard Scan
- Enhanced Scan

If the enhanced scan is selected, a further option to "save captured text" is available.

### Supported file types

- .DOCX
- .PPTX
- .XLSX
- .PDF
- .CSV
- .TXT


## Read Websites

The enhanced web page reader presents 2 options

![image](images/enhancedWebReader.png)<br>

- Standard Scan
- Enhanced Scan

If the enhanced scan is selected, a further option to "save captured text" is available.



## Scanning documents


### Existing matches
If another users has read the enhanced scan against the same document or web page, the NLP scan will not run again.   Instead the 

![image](images/ExistingMatches.png)<br>


## Insight results

### Attachment card
Potentially 2 new icons will be shown on the attachment card within the workspace canvas.

![image](images/AttachmentCard.png)<br>

- the text icon is shown if the text from the document or web page has been saved
- the eye icon is shown if the enhanced scan was selected and new "insights" are available

### Viewing insights
To view the insights

- Select the associated attachment card within the canvas
- the text and insight icons are shown within the right hand information panel<br>
![image](images/InformationPanelWithInsights.png)<br>
- select the "Insights" icon
- The insights canvas is now shown<br>
![image](images/InsightsCanvas.png)<br>

### The Insights Canvas

![image](images/InsightsCanvas2.png)<br>

Within the insights canvas you have the following options:

- Filter based on the type of insight (linked entity, key phrase, named entity)
- Insight Category
- Show saved text
- filter based on free text entry
- sort by occurrence
- sort by insights included within other users workspaces

#### Sort by insights included within other users workspaces

Insight cards which have been added by other users to their main workspace canvas include a "graph" icon within the card.

![image](images/InsightCard.png)<br>
![image](images/OtherWorkspaces.png)<br>


#### Adding insights to your main workspace canvas

![image](images/InsightCard.png)<br>

Select the (+) icon within the insight card to add the insight card to your main workspace canvas

## Text viewer

If the option to save the text during the initial scan was selected the raw text is available to be viewed.  Within this view you can select any of the matched insights 

![image](images/TextViewer.png)<br>

Within the text view you have the following options: 

- highlight insights by name (list or free text search)
- View insight canvas


### searching and text highlights

![image](images/HighlightedText.png)<br>

The selected text is highlighted within the document text and you can also click to jump to any other page where the text is included.


![image](images/TextPages.png)<br>

:bulb: The text pages are defined by 5000 characters sections from the original document and do not represent the actual pages within the original document


---

Usage of insights within the other workspace features

- Included within the graph and compare views


Updates to be made to

- heatmap view
- download to csv
- send to