# Moodle Database: Educational Data Log Analysis
## Overview
This week we analyse the 2019 10 Academy learners activity in the Moodle Learning Management System. The moodle LMS is a highly scalable framework, and all students activities are stored in a highly structured database.  
## Business Need
Many educational facilities such as colleges, universities, bootcamps rely on scalable and versatile Learning Management Systems. 

The Moodle LMS  is a free and open-source learning management system written in PHP and distributed under the GNU General Public License. It is used for blended learning, distance education, flipped classroom and other e-learning projects in schools, universities, workplaces and other sectors. With customizable management features, it is used to create private websites with online courses for educators and trainers to achieve learning goals. Moodle allows for extending and tailoring learning environments using community-sourced plugins.

In 2019, 10 Academy used the Moodle LMS to manage about 1000 students in their 6 months data science training. Learners, course instructors, and all admins interacted with the Moodle system for almost all the training activities. All events from these activities are logged in the moodle postgres database. 

10 Academy, like any other educational facility, is interested to understand the learners skill and knowledge development, and is interested to build models that are able to predict possible dropouts as well as classify learners into doing, well, doing ok, and struggling groups. 10 Academy is also interested in automating the process of reminding learners approaching deadlines, providing quick feedback based on their overall community engagement and performance. Moreover, given the main goal of 10 Academy training is to make students job ready, it wants to measure students' performance across many relevant metrics. 

**Challenge:** To explore the 10 Academy Moodle logs stored in the database together with many other relevant tables. By the end of the analysis, we will build a Tableau dashboard that illustrates the progress of students across time.

## Challenge Approach
The tasks are divided into four sub-tasks
1. Moodle database schema understanding
2. Data Extraction Transformation and Loading (ETL)
3. Dashboard making with Tableau
4. Automation and Deployment

Task 1 and task 2 are handled in the jupyter notebook provided.

You can find the public tableau dashboard [here](https://public.tableau.com/profile/anastasia.kiiru#!/vizhome/education_log_analysis/Dashboard1?publish=yes)