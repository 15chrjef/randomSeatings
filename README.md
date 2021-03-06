Seating Chart Generator


DESCRIPTION:
Teachers often want to make seating charts that assign their students to tables.
Imagine ClassDojo is implementing this as a feature. In particular, we'd like
to assign students to tables such that no table has "all the troublemakers" or
"all the teacher's pets".

Your task is to take an array of integers (each representing a student's point
total) and a number of groups, and assign the students to groups such that
each group is of the same size (or nearly so) and the average of point totals
across each group is approximately the same.

SPECS:

  * Your script
    - Takes two arguments:
      * The first argument is the number of groups required.
      * The second argument is a comma-separated list of integers, each
        representing a student in the class. The integers may be negative.
        The list will be sorted in ascending order.
    - Should log each group on its own line to stdout.
    - Each group should consist of a space-separated list of integers.

  * Requirements
    - Your goal is to minimize the standard deviation of the group averages.
      To put it another way, your group averages should be as close together
      as possible.
    - Group sizes should differ by no more than 1.

  * Evaluation
    - Our evaluation script (run.py) will call your script and score its output.
    - Make sure your script is executable! This depends on language. For example,
      it may need to begin with a 'shebang' (something like #!/usr/bin/env node 
      or #!/usr/bin/env python)
      If you see an error like `OSError: [Errno 8] Exec format error`
      this is because you haven't se the `shebang` properly.
    - The default settings use 24 students and 6 groups, without skew.
    - Your solution need not be optimal, but should have 'reasonable'
      performance across a variety of inputs and run in a 'reasonable' time.
    - Use the `--help` flag to view available options.
    - Use the `--log` flag to run your script without evaluating the score.
      This is useful for debugging.
    - example usage: `./run.py solution.rb`
    - for java, run `./run.py java/java.sh --log --students 40 --groups 6` where java/Solution.java is your implementation

EXAMPLE:
  
  * Input:  
    4 1,2,3,4,5,6,8,9,10,11,12

  * Output:  

    1 8 10
    2 6 12
    3 7 9
    4 5 11

  * Evaluation:  

    Group Averages: 6.33 6.66 6.33 6.66  
    Standard deviation of group averages: 0.190526

