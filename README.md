# Lightning Universal Lookup Component
## Powerful lookup component for your developments

Boost the development of your custom components with a new powerful lookup component. It looks like a standard one, pretty easy to customize and works everywhere – even in Salesforce1.

It look like standard field and could be used with Standard and Custom Objects.

  <p align="center">
    <img width="550" src="https://image.ibb.co/fW4q2Q/ezgif_com_video_to_gif_1.gif" alt="showLastViewed">
  </p>

### Installation

<a href="https://githubsfdeploy.herokuapp.com">
  <img alt="Deploy to Salesforce"
       src="https://raw.githubusercontent.com/afawcett/githubsfdeploy/master/deploy.png">
</a>

Optionally, you can install it as <a href="../lastworking">unmanaged package</a>.
Also available as <a href="">managed package on AppExhange</a>.

### How to use it

Custom Lookup component field has 5 attributes.

Main attributes:	
  * objectType - API name of Salesforce Object. Could be Standard or Custom. 
  * selectedRecordId - variable that will contain Id of selected record.

Optional attributes:
  * label - label. Default is label from Object.
  * showFiveRecent - feature from standard lookup field, showed 5 recently viewed records. Default is true.
  * widthPX - width of field. Default is ‘300px’.


```html
<aura:attribute name="selectedId" type="String"/>

<l_lookup:Lookup objectType = "Account" 
                 label = "Customer"
                 selectedRecordId = "{! v.selectedId }"
                 readOnly = "false"
                 showFiveRecent = "false"
                 widthPX="400px">
</l_lookup:Lookup>

```
