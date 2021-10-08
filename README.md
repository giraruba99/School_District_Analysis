# School_District_Analysis
## Overview and purpose of the project
   * Purpose- The main pupose of this analysis can be summarized as:
     - To run a comparative analysis of Thomas High School (THS) by ommitting 9th grade math & reading scores
     - To repeat the analysis of the whole school district with ommited THS 9th grade scores
     - To determine if the suspected acadamic dishonesty really existed, and detemire how much this suspected unethical behavior affected the overall school performance
     - To provide the school district board a scientific data on which they can compare both sets of data and decide accordingly
   * Overview of the project- The overview and analysis methedology followed can be summarized as follows:
     - As mentioned above, the purpose of the analysis is to determine if THS 9th grade reading and math was altered. Thus with the loc. method, we run a comparison operator to filter out the targeted school and grade.

![THS comparison operator](https://user-images.githubusercontent.com/89214854/136459887-f39e1337-34e3-42da-8611-9901268d6edf.png)

    * Nullified THS 9th grade scores
     
     - Once we select THS 9th grade, we used the same script to nullify the scores and replace them with NaNs. The reason behide the technique is to take out the effect of the suspected score out of the data and rerun the whole analysis again. The following image shows THS 9th grade math and reading score replaced by NaNs.

![THS with 9th grade NaN](https://user-images.githubusercontent.com/89214854/136459925-c375714d-beee-4223-8b12-99f0d6031fe2.png)


## Result

   * District Summary Results
     - As expected, the new school district overall passing percentage went down after the refactored analysis. Surprisingly though, it was only obout 0.3%, which is not a big swing. But, we are not there yet, we can not for sure say minimal effect until we run all the rest of the analysis.
![District summary DataFrame](https://user-images.githubusercontent.com/89214854/136460072-1a733afd-d86d-4fd1-941a-e86eba2a0573.png)

   * School Summary Results
     - We also rerun the analysis to see all schools individually, if THS overall passing was affected by a lot. As observed above in the district summary, THS overall passing went down by only 0.4% points. Yet, we are oveserving a downward movment of THS oveall passing.

![School summary DataFrame](https://user-images.githubusercontent.com/89214854/136460334-4f310af6-de49-4761-af70-7a0f1259d052.png)


   * Results of top 5 schools
     - THS is no more among the top 5 hightest performing school. The small downward movment of the overall passing percentage knocked down THS from the top 5 schools. The main reason for this looks like, all the schools performances are very close to one another and a small shift will alter in their overall rank.

![Top 5 schools](https://user-images.githubusercontent.com/89214854/136460113-e08c534f-3e84-4e92-b52e-4b90d58d75d1.png)


   * Result of 5 bottom schools
     - This category didn't change after we rerun the analysis as THS is still towards the top of the list.

![Lowest 5 schools](https://user-images.githubusercontent.com/89214854/136460145-717dfe67-e762-47f7-a1fe-fd083dc62ab7.png)

   * Math scores by grade
     - The image below clearly show there is nothing to report on 9th grade math score for THS
     
![math score by grade](https://user-images.githubusercontent.com/89214854/136619972-b3f269e6-e30b-4157-bd18-f1864a93b6a9.png)

   * Reading scores by grade
     - The following image is reporting the null valu for THS grade 9 scores

![reading score by grade](https://user-images.githubusercontent.com/89214854/136620029-496a27c7-9f91-4850-bd35-b6afc87fac4e.png)


   * Results by student budget
     - The main swing in overall passing range was seen in the range of $630-$644 *. Overall passing rate went down from 62% to 56%.
     
![per student budget](https://user-images.githubusercontent.com/89214854/136460283-e50ef19b-8144-4a22-aab6-3ff8f19b668c.png)

   * Results per school size
     - Medium sized schools (1000-2000) get affected by reruning the analysis, because THS falls with in this category. 

![per school size](https://user-images.githubusercontent.com/89214854/136460395-6229e5b0-31f1-422f-8285-873077003e5c.png)

   * Results per school type
    - The overall passing percentage of charter schools went down from 90% to 87%, a clear indication that removing THS 9th grade scores affected the overall passing rate in charter schools.

![per school type](https://user-images.githubusercontent.com/89214854/136460428-1414b7e0-7523-4e2c-923e-3ca6489bd545.png)


## Summary and Conclusion
  * It can be summarized that removing 9th grade scores from THS affected the overall results in areas of the analysis. 
  * But, we did not find a big evidence to conlude there was an acadamic dishonesty to a level that needs special attention. Because:
       - Regardless of how great/bad the reading and maths scores are, by replacing them with NaNs we are going to swing the whole analysis anyway.
       - The method we used is inconclusive to determine the suspected misbehavior of the school.
       - Thus, we can not conlude there was altered score with the tools at hand

## Recomendations
   
   * If we need to continue our adventure of data analysis, and we want to keep looking other factors before we conlude the unethical behavior, we need:
        - Compare 9th grade scores of THS with other schools, and look how they fare
        - Looks back 9th  grade score of THS for consecutive years and loom how they fare
        - Continue monitoting next year how will they fare in relation to other schools and other grades of the same school
    


