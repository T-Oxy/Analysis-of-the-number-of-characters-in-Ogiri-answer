# Analysis-of-the-number-of-characters-in-Ogiri-answer
## Intro
I investigated the question “Is the funny Ogiri’s answer less (or more) characters?”. 


Ogiri (Japanese word: “大喜利”) is the game where people answer questions comically. Of course, which answer you find interesting is different for each person, but there are certainly answers that are appealing to many people and those that are not. The humorous answers are often characterized by their rich creativity and good word sense. 
In addition to that, there are a certain number of opinions that "the number of characters in the answer is important". I thought that I can get a simple trick to improve Ogiri skill if this opinion is correct. This is because adjusting the number of characters is much easier than developing creativity and word sense.

So, in order to solve the question presented at the beginning, the following experiments were performed.

## Experiment Design
1. Dependent variable: RATE.
    
    RATE has two levels, “high” and “low”. RATE means people’s evaluation of each answer of Ogiri. The answer of RATE=“high” is considered interesting, and the answer of RATE=“low” is considered uninteresting.
2. Independent variable: LEN. 
    
    LEN is the number of characters in Ogiri's answer (= answer string length).

3. Hypothesis:
    
    I would like to test the differences between the mean value of LEN of the answer with RATE=“high” (=μ1) and that with RATE=“low” (=μ2). So the test hypotheses is shown below.
    - H0 (null hypothesis):     μ1 = μ2
    - H1(alternative hypothesis): μ1 ≠ μ2
4. Experiment parameter: 
    - Desired significance: α = 0.05
    - Desired power: (1 – β) = 0.8 
    - Effect size: d = 0.8
5. Sample size calculation:

    Based on the parameter values above, I calculated the sample size(=n) required for the paired two-sample t-test (two-sided test). Caluculation result is n=25.525. So I decided the sample size to be n=26.
6. Data collection protocol:

    In this experiment, I choose the homepage called “bokete”(https://bokete.jp/) as the data cource. “Bokete” is a service in which users post images and characters to make them "themes", and multiple users post funny answers to the themes to laugh and enjoy humor. People also can be evaluated by voting for interesting answers.

    1.	Randomly select 26 themes from “bokete”.
    2.	Select one answer with the most votes for each theme as the answer with RATE = "high", and count the number of characters in the answer to find LEN.
    3.	At the same time as 2. , select one of the answer with few votes for each theme as the answer with RATE = "low" to find LEN.

    So in each theme, one answer with RATE = "high" and one answer with RATE = "low" are paired. Collected all data are saved in a csv file.

7. Data analysis protocol:
    1.	Create a boxplot with two axes, RATE and LEN, based on LEN values received from the csv file.
    2.	Calculate the confidence intervals for the values observed for LEN. The confidence level is 95%.
    3.	Plot the mean and confidence intervals of LEN together
    4.	Perform the paired two-sample t-test (two-sided test)  and consider the hypothesis(H0, H1) that was made.


8. Data Collection
    
    I collected the necessary experimental data according to the above data collection protocol. The data file name is “bokete_len_data.csv”. 
