# Applying predictive maintenance to debugging approaches in collaborative robots.

Industrial robots running in a production line have varying lifespans depending on the stress they endure. New research have unlocked methods of predicting the lifespan of a robot based on the program that it is executing. While programmers might have knowledge that programs cause stress, the exact extent of this stress is not easy for programmers to know.
Adapting a program to extend lifetime must take into account the effect on cycle-time. As such it is important to empower the developer with the knowledge of exactly _where_ and by _how much_ the robot is being worn out by the program.

We will be investigating whether an extension of the existing work can create a more efficient workflow for the developer resulting a better result.
## Scope of work:
The project will focus on extending and enhancing a debugging tool visualizing bugs and errors in URScript code. The extended features include: 
1. Calculating "impact scores" for each line in the provided program. 
	- Increase usability of the tool by highlighting lines with higher impact on the robots lifetime. 
2. Tracing robot path, visualizing areas that impact robot lifetime negatively. 
3. Enabling the tool to run in real-time on a robot

### Methods:
1. **Combine EDDE research with Joint Stress Estimation:** Use the existing research of joint stress estimation for which parts of the run that provide the most stress with the EDDE research to highlight which lines cause the most stress.
2. **Evaluation & Analysis:** Evaluating whether the tool extension leads to 
	- a Faster cycle times with the same expected life-time
	- b Longer expected life-time with the same cycle-time
	- c Faster arrival at the extended life-time and/or faster cycle-time than using only the existing tools.
3. **Interactive Visualizations:** Creating interactive visualizations should aid the speed of the developer.


## Expected outcome:
We expect to contribute with new knowledge about how stress visualizations can lead to more efficient programs and extend the life of the robots.


# Timeline

```graph
gantt

    title Engineering research in software

    dateFormat DD-MM-YYYY

    axisFormat %d/%m-%Y

    section Project preparation

        Project definition          :a1, 10-02-2025, 7d

        Initial scoping    :a2, after a1, 7d

        Find existing tools and knowledge :after a1, 7d

    section Project work

        Calculate impact scores :p2, after a2, 21d

        Show stress on path :p2, after p1, 14d

        Enable real-time monitoring :p3, after a2, 14d

  

    section Evaluation

        Design evaluation :e1, after p2, 14d

    section Paper writing

        Write paper :after e1, 21d
```