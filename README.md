# ArcGIS Field Maps: Using Arcade to build smarter maps and forms
This is the repository with Screenshots and Arcade code that was used during the tech-session at the European Developer Summit 2024 in Berlin.
### Session description
Mobile workflows can be streamlined and made smarter by combining ArcGIS Field Maps with Arcade. This session will focus on the how Arcade can be used within the map to provide an intuitive experience when exploring data and how it can be used to configure smart forms for data capture. As well as showing examples the session will also share advanced Arcade patterns and best practices for use in the Field.
## Symbolgy with Arcade
![image](https://github.com/user-attachments/assets/5ac2e081-f0be-4c1f-928a-e4ca08b9d8b8)
![image](https://github.com/user-attachments/assets/af6faa70-6640-4e19-bda4-02b0fd6ad311)
The Arcade-code for the in the symbology used expression can be found here:
https://github.com/chgresri/arcgis-field-maps-using-arcade-to-build-smarter-maps-and-forms/blob/d1941323f0e89e8bcf3871fd385ac2b9621f2a42/arcade-symbology
## Labels with Arcade
![image](https://github.com/user-attachments/assets/63a31047-03ff-4ef2-a2e4-cb62ad76fb11)
![image](https://github.com/user-attachments/assets/c0a47dec-50eb-467e-b5f2-bac2c2ff5850)
The Arcade-code for the in the labels used expression can be found here:
https://github.com/chgresri/arcgis-field-maps-using-arcade-to-build-smarter-maps-and-forms/blob/0e595115050ab2b33c81fb16216dacd4eccb7b3e/arcade-labels
## Popups with Arcade
### Popup settings for the Boundary Layer of the Swiss Nationalpark
![image](https://github.com/user-attachments/assets/69ee6bb8-fae8-4d21-9673-505e38faebeb)
![image](https://github.com/user-attachments/assets/a7707cbc-0002-4ca0-93d9-30b0b57863d8)
![image](https://github.com/user-attachments/assets/a622fa46-f109-4162-85b4-2e610652f1ce)
The same Arcade expression logic was used for all the attributes that should be used in the bar chart in the popup. So, one has to create several Arcade expressions which point to a different attribute value (in this use case it was the tree health issue type). The Arcade code can be found here:
https://github.com/chgresri/arcgis-field-maps-using-arcade-to-build-smarter-maps-and-forms/blob/9023fce1bc87373ed1fdea3ea031683686f7cf78/arcade-popup-boundary-layer-nationalpark
### Popup settings for the Tree Health Observations
![image](https://github.com/user-attachments/assets/02d492bb-a8ae-4211-85f9-0ca23a0dc60a)
#### Text Block settings:
![image](https://github.com/user-attachments/assets/f260ff5c-4809-4974-88c4-95762f82a397)
![image](https://github.com/user-attachments/assets/5f58fc03-d3a0-4006-91b7-33fecbda8d8a)
##### Arcade Expressions for the Text Block:
![image](https://github.com/user-attachments/assets/8ba5b31b-63dc-4ca1-99fa-65a0c17bce7c)
![image](https://github.com/user-attachments/assets/a69942e0-8ace-4b14-b156-5420bcaf44ac)
The Arcade code can be found here:
https://github.com/chgresri/arcgis-field-maps-using-arcade-to-build-smarter-maps-and-forms/blob/c65ad7f933da07dc26717fece3380ef1ae046a4f/arcade-popup-expression-1-tree-observations-text-block
![image](https://github.com/user-attachments/assets/96d99a6a-77bb-4c9a-a8d4-669b313e91f6)
The Arcade code can be found here:
https://github.com/chgresri/arcgis-field-maps-using-arcade-to-build-smarter-maps-and-forms/blob/7b92de3ec7cdfc5ffafc9da0bec822f279a54b42/arcade-popup-expression-2-tree-observations-text-block
#### Arcade Block settings:
![image](https://github.com/user-attachments/assets/227a0c80-320f-49f4-8fa1-578a50812037)
The Arcade code can be found here:
https://github.com/chgresri/arcgis-field-maps-using-arcade-to-build-smarter-maps-and-forms/blob/491da263fc5db62fe36c9b74bfe9d0c767240ada/arcade-popup-tree-observations-arcade-block
## Form in the Field Maps Designer
In the Field Maps Designer on the form for the Tree Health Observations, the following groups were created and filled with attributes:
![image](https://github.com/user-attachments/assets/1bd829f0-2886-4d5f-bcd7-0fa505aae037)
### Group: General Information
Two attributes were set as required and a Info Text Box was included for information.
![image](https://github.com/user-attachments/assets/cdf20eb7-55fd-4097-8c7e-5e6bf46750e0)
### Group: Detailed Observation
Nothing special was set in this group. All the 4 attributes contain list values to select.
![image](https://github.com/user-attachments/assets/1ea45841-e3ab-47b0-9bff-4239eb90186b)
### Group: Information on Pest
This group is conditionally visible. It contains two attributes from which one is conditionally required.
![image](https://github.com/user-attachments/assets/4391a42e-c9f5-4ae1-af99-eee5b07f39cc)
#### Conditional visibility:
![image](https://github.com/user-attachments/assets/5e74e00e-259d-4dff-b502-75cd380b3d06)
The Arcade code can be found here:
https://github.com/chgresri/arcgis-field-maps-using-arcade-to-build-smarter-maps-and-forms/blob/d4e377cc6d5e4ce52a6fe5ca46efb703d37c0702/arcade-form-conditional-visibility-group-information-on-pest
#### Conditionally required:
![image](https://github.com/user-attachments/assets/97b9b645-824b-41ad-a1bf-e80d190bd7dd)
The Arcade code can be found here:
https://github.com/chgresri/arcgis-field-maps-using-arcade-to-build-smarter-maps-and-forms/blob/af390ec65672310cb3028f72ef4806fe81729e03/arcade-form-conditionally-required-group-information-on-pest
### Group: Information on Leaning
This group is conditionally visible. It contains one attribute, which is conditionally required.
![image](https://github.com/user-attachments/assets/2e81abdc-cd31-40a0-80b5-4b2f8747280a)
#### Conditional visibility:
![image](https://github.com/user-attachments/assets/8d1f7859-497f-432f-ae4b-7cb6c0a70621)
The Arcade code can be found here:
https://github.com/chgresri/arcgis-field-maps-using-arcade-to-build-smarter-maps-and-forms/blob/513ff950b8f9edfc7db1598a425926571c9440ce/arcade-form-conditional-visibility-group-information-on-leaning
#### Conditionally required:
![image](https://github.com/user-attachments/assets/db9c9a08-5e07-4863-811e-87e6c8a0a98e)
The Arcade code can be found here:
https://github.com/chgresri/arcgis-field-maps-using-arcade-to-build-smarter-maps-and-forms/blob/1c892cada49ce971e2dc1c44bce40d74e1ea8316/arcade-form-conditionally-required-group-information-on-leaning
### Group: Information for Hikers
This group contains a Info Text Box that is conditionally visible and includes attribute values and a arcade expression. Furthermore, it contains a required attribute and an attribute, that is calculated by an arcade expression and thus, read-only.
![image](https://github.com/user-attachments/assets/8fecd19b-d931-4347-a3b2-31560afd5f88)
#### Info Text Box:
![image](https://github.com/user-attachments/assets/7a80818a-8f0c-4789-be22-d44e1113f1c2)
##### Arcade expression in Info Text Box:
![image](https://github.com/user-attachments/assets/d1b4bdbd-a1e2-4b71-ad7c-7e1ae81030be)
The Arcade code can be found here:
https://github.com/chgresri/arcgis-field-maps-using-arcade-to-build-smarter-maps-and-forms/blob/60d1c25b923d4adc4fab0d0a436bd39477a3dc98/arcade-form-info-text-box-expression
##### Conditional visibility:
![image](https://github.com/user-attachments/assets/82bf9c24-fc61-4038-8c43-6e40ea324658)
The Arcade code can be found here:
https://github.com/chgresri/arcgis-field-maps-using-arcade-to-build-smarter-maps-and-forms/blob/23e44b9240e7840b7a26af91a887c082ed6de799/arcade-form-info-text-box-conditional-visability
#### Calculated expression for attribute Risk for hikers:
![image](https://github.com/user-attachments/assets/194f7f48-2802-420a-bd1b-bb07d04b117e)
![image](https://github.com/user-attachments/assets/77ed54a6-f1aa-4717-94f0-2746fe1e6685)
The Arcade code can be found here:
https://github.com/chgresri/arcgis-field-maps-using-arcade-to-build-smarter-maps-and-forms/blob/d57ada32295fcfdc59cea6c1095ea78c17ab91c5/arcade-form-calculated-value-expression-risk-for-hikers
### Group: Treatment Information
This group has a switch-button attribute and a date attribute, which is calculated by the arcade expression: "Now()" and is only visible if the switch button is activated.
![image](https://github.com/user-attachments/assets/179baf74-5e4d-4c50-827b-dc8401b778cc)
#### Conditional visibility:
![image](https://github.com/user-attachments/assets/bc5b1241-5502-4e59-8876-5abf5889aecd)
The Arcade code can be found here:
https://github.com/chgresri/arcgis-field-maps-using-arcade-to-build-smarter-maps-and-forms/blob/db35a0b54abe91776e4985d1623a18615ff7b77e/arcade-form-conditional-visibility-treatment-information-group-treatment-date
## Geofences in Field Maps Designer
### Location Notification:
![image](https://github.com/user-attachments/assets/b82e1032-5f1c-4c7e-9a6c-1541d358139e)
### Location Sharing:
![image](https://github.com/user-attachments/assets/986ec576-5e1e-49fa-b12f-2e8003c4e661)
#### Arcade expression for conditional Location Sharing:
![image](https://github.com/user-attachments/assets/1d08b7bb-e179-402d-9e11-aa3b7c8e6ff1)
The only Arcade code part the was added is: " && Hour(Now()) <= 9 && Hour(Now()) > 17".
