# class-scheduler

**Find out how to best fit all your courses into your schedule across multiple semesters**

Enter courses in the format ("course_name", course_credits, [potential_semesters], [prerequisites]. Ensure the course names and semster names do not have a "_" (underscore) character. This is not checked, but will cause the program to fail using z3.

Enter the semesters in the format (semester_name, max_credits_this_semester). All semesters that exist in the courses list must be in the semesters list. Put the semesters in order if listing prerequisites.

z3 generally runs slightly faster than max flow and has greater functionality (ie. nonsingular courses). Augmented z3 is the only function that works with prerequisites, but does tend to run longer.

*Ported from https://gist.github.com/shreykshah/094b83eca043d96b08f8e9dc49b8ba17. For best experience, open in [Google Colab](https://colab.research.google.com/gist/shreykshah/094b83eca043d96b08f8e9dc49b8ba17/class_scheduler.ipynb).*
