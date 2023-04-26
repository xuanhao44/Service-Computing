# Exercises - Case study

Pick one domain or industry - almost any domain or industry is fine – it is better not to choose the construction industry.

Find several cases of how service orientation was used by companies in this domain/industry.

- You should find case descriptions on service provider websites. The cases should be from different providers. You can also find relevant research papers. You can choose Chinese companies and/or Chinese service providers as your examples, but your report should be in English.

Study the cases you found, review how the cloud is used in this industry, and identify the important aspects of using cloud technology in this industry

- Use cases 
- Benefits
- Challenges
- Other issues you can study:
  - Examples of SaaS, PaaS, IaaS, XaaS in this domain/industry
  - Popular cloud deployment models in this industry: public/private/hybrid/… and the reasons behind it
  - Recommendations and steps to be taken by companies in this domain/industry to solve their problem using cloud computing technology

Your report should have a title in the following format: “Service orientation in ________ domain/industry: use cases, benefits, and challenges.”

Submit to the Blackboard by April 16th

## Service orientation in metro industry

Tokyo Metro Co., Ltd. is a company that operates nine subway lines in Tokyo, Japan.  The company was established in 2004 as a result of the privatization of the former Teito Rapid Transit Authority (TRTA).  Tokyo Metro Co., Ltd. has been using cloud technology to improve its business operations and customer services.

### Use cases, Benefits, Challenges

Reference: https://customers.microsoft.com/en-us/story/1584832935479879254-tokyo-metro-travel-transportation-azure-en-japan

|                   | Use case                                                     | Benefits                                                     | Challenges                                                   |
| ----------------- | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| Title             | Use AI to help Track Abnormality Detection and Power Apps to develop a mature solution | Auto process(Improved efficiency)                            | Difficult to detect abnormal rail fasteners **directly** from the images of tracks |
| Short description | Microsoft helped Tokyo Metro improve the quality of inspections by providing AI services and tools. Tokyo Metro used Microsoft Azure AI services and Microsoft Power Platform to create a solution that detects equipment deterioration and other abnormalities from images taken of railroad tracks. | Tokyo Metro has created an excellent detection model and classification model, as well as an application that calls the detection model and an application that determines normality/abnormality based on the classification model. However, handover from the detection model to the classification model had been performed by manually cropping images. <br/>It was very time-consuming to do this manually every time. Therefore, Microsoft created codes to automate this process, that is, linking everything together, so that the codes would be called from the application and output could be checked on the display screen. | A model was created using Custom Vision, an image recognition service provided by Azure, to detect only abnormal rail fasteners from the photographs of tracks. With the model, it was difficult for Microsoft to determine the difference between normal and abnormal rail fasteners, and the model did not provide sufficient detection accuracy.  <br/>An image model for detecting rail fasteners themselves is to be created first. Then, only rail fasteners are to be cut out of the images, followed by classification into normal and abnormal fasteners. In other words, we propose to create a model to detect abnormal fasteners with high accuracy, by dividing the process into three steps. |

### Recommendations and steps to be taken by Tokyo Metro Co., Ltd. to solve their problem using cloud computing technology

*Still use the use case mentioned above*

**Strong motivation**: Although it is hard to proceed with innovation in track maintenance, the employees still had a strong will to apply AI and cloud computing in this specific area.

**Get help from IT**: They have an established culture of getting hints from the IT department about the potential application of new technologies and then putting them into practice based on distinctive knowledge unique to the field. Their IT department suggested the AI services of Microsoft Azure (hereafter, Azure), namely Azure Cognitive Services and Microsoft Power Apps (hereafter, Power Apps).

**Clear objective**: From the very beginning, Tokyo Metro’s objective was clear — detecting abnormalities on rail fasteners from images.

**Problem**: **The initial model created by Microsoft was not good enough to use**. At that time, a model was created using Custom Vision, an image recognition service provided by Azure, to detect only abnormal rail fasteners from the photographs of tracks. With the model, it was difficult for Microsoft to determine the difference between normal and abnormal rail fasteners, and the model did not provide sufficient detection accuracy.

**Solution by Tokyo Metro Co., Ltd.'s employees**: It is quite difficult to detect abnormal rail fasteners directly from the images of tracks. Therefore, an image model for detecting rail fasteners themselves is to be created first. Then, only rail fasteners are to be cut out of the images, followed by classification into normal and abnormal fasteners. In other words, we propose to **create a model to detect abnormal fasteners with high accuracy, by dividing the process into three steps**.

**Create better model by employees themselves**: They had a firm grasp of the effective way of using AI — it is all right to improve the accuracy through a trial-and-error process, using Custom Vision. As a result, the accuracy of the model they created was much higher than 90% while the accuracy of the model Microsoft created was about 70%.

**Create auto apps with the help of Microsoft**: After repeated meetings, they were finally able to develop an app that worked well. The development was easy in general while they asked for Microsoft’s assistance when they needed to write some code.

"**Accumulated data is to be utilized in machine learning and visualized with BI tools, for preventive maintenance and inspection decisions**." The company agreed that this would be the main process to solve their problem using cloud computing technology.