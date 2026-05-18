# CSC590-FinalProj
In order to execute the above models. It is important that you also have the datsets, each model was training on. The physician network JSON schema was provided in this repository as well as the predictions pickle file. The lymphocyte detection datset however, was too large to put in this repository therefore in order to run the lymphocyte model you must go to https://cedars.nationalcampus.ai/project/30/ and download the dataset from there. 

Upon executing the code, you will see the comparison between Graph Neural Networks and traditional network analysis models 

Model 1: Physician Dataset Network



<img width="707" height="422" alt="PhysicianGNN" src="https://github.com/user-attachments/assets/527c7218-383b-4185-9815-16ae7186f7eb" />


With the first dataset focused around physicians adopting a new technology, one of the best results I gathered was a MAE of 3.39, a MSE of 15.27, and a RMSE of 3.91. When put against a Linear Regression model, it outperformed the LinReg model by predicting closer to the actual year by 1 year and on average, made a major mistake that was half of what LinReg made. When viewing the results, this showed that my GNN model performed better on understanding the connection between physicians and how they adopted new technology based on their connections with other physicians.

Model 2: Fake News Detection


<img width="660" height="388" alt="FakeNewsGNN" src="https://github.com/user-attachments/assets/01485ab3-29ef-4d87-ba5a-d746ca74c549" />


When completing my model for my Fake News Detection task, the best results I gathered for my model was an accuracy of 92%, with a precision of 92%, a recall of 0.94, and a F1 of 0.92. When the logistic regression model was executed right after my model trained and tested the dataset, it recorded an accuracy of 77%, with a precision of 76%, a recall of 0.78, and a F1 of 0.77. These results, which are compared side by side, showed that the graph was playing a significant role in helping my model discover the underlying patterns within the small dataset in comparison to Logistic Regression. Without the attributes that were present in each node, Logistic Regression could not efficiently predict the test data for the UPFD dataset.

Model 3: Lymphocyte Detection


<img width="710" height="430" alt="LymphocyteGNN" src="https://github.com/user-attachments/assets/b77e1255-a3c1-46c1-99c5-a699a4c31bd7" />


For my final model that focused on detecting if a cell in an image was immune or non immune, my best results gathered an accuracy of 61%, with an AUC of 0.83, precision of 72%, recall of 0.69, and an F1 of 0.70. In comparison to the Multilayer Perceptron Model, that gathered an accuracy of 60%, AUC of 0.61, a precision of 51%, a recall of 0.53, and a F1 of 0.52, my GNN model completely outperformed the MLP model in detecting immune cells for all the graphs that were present. With the incorporation of the network into my model, it was able to understand the underlying patterns of the connections between nodes for immune cells.



Disclaimer: Although this was my standard results upon performing the final presentation for the CSUDH National AI Campus on May 13, 2026, after the presentation I tried to change my code in order to get better results by changing how the training graph and testing graph were split and how the data was put into the network. I believe that I could create a GNN model with better results than what I was gathering before the presentation, and upon working on the code before this final report was due, I ended up hindering my model to where it now underperforms in comparison to the MLP model. For the sake of transparency and integrity, I will share my current GNN model results so it does not seem I tried to cover what my current GNN model is evaluating.



<img width="750" height="450" alt="Screenshot 2026-05-18 033527" src="https://github.com/user-attachments/assets/7e318f10-3350-4517-9263-d2bcaec844d8" />
