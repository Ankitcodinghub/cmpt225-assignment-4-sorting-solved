# cmpt225-assignment-4-sorting-solved
**TO GET THIS SOLUTION VISIT:** [CMPT225 Assignment 4-Sorting Solved](https://www.ankitcodinghub.com/product/cmpt225-assignment-4-sorting-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;120195&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CMPT225 Assignment 4-Sorting Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
The ability to destroy a planet is insignificant next to the power of sorting. — Darth Vader (if he was a computer scientist)

Your task is to run performance experiments on these sorting algorithms:

bubble sort insertion sort selection sort shell sort (see below)

merge sort quick sort

iquick sort (see below) priority queue sort where the priority queue is implemented as a heap

You’ll create a spreadsheet to report on your results (described below).

Put your implementations of all the functions in a file named a4_sort_implementations.h. Implement each algorithm as described in the textbook/notes: you can use the code from the textbook, or from other sources (make sure to cite your sources!). Implement the exact function headers listed in a4_base.h. Don’t change a4_base.h in any way: put all the sorting-related code you write in a4_sort_implementations.h.

Important The only #include that a4_sort_implementations.h can use is #include “a4_base.h”. No other #includes are allowed.

Shell Sort

Shell sort is a sorting algorithm that works by swapping pairs of elements in ever-decreasing gaps. The sequence of gaps has a significant impact on the algorithm’s performance, and so for consistency you are required to use this gap sequence: n/2, n/4, n/8 …, 1 where n is the size of the vector being sorted.

This means that the last gap will always be 1, and so the algorithm will always finish with a final pass of insertion sort.

Important There are gap sequences that make shell sort run more efficiently than this one, but, for the sake of consistency, do not use them. Use only the gap sequence given above.

iquick Sort

iquick sort is regular quick sort, except when the sub-vectors being sorted are shorter than some predetermined threshold length (that you pick), insertion sort is used to sort them instead of quick sort. If you choose a good threshold length, you can get better average-time performance than regular quick sort. Do some experimentation to find the best threshold length!

Priority Queue Sort

Testing Your Implementations

Test your implementations using test_sorts.cpp. You can modify that file in any way you like (it is not one of the submitted files for this assignment).

Note test_sorts.cpp only checks for basic correctness of the sorting algorithm, and ignores the Sort_stats objects they return. Feel free to add more test cases if you want to test the Sort_stats objects.

Notice that most of the functions in a4_base.h are template functions, i.e. they take a vector&lt;T&gt; as input, where T is a type of value that can be sorted.

All the sorts return a Sort_stats object containing their running time and comparisons counts: “`cpp // a4_base.h

// …

typedef unsigned long ulong; struct Sort_stats { string sort_name; size_t vector_size = 0; ulong num_comparisons = 0; double cpu_running_time_sec = 0.0;

string to_csv() const

{

return sort_name + “, ”

+ to_string(vector_size) + “, ”

+ to_string(num_comparisons) + “, ”

+ to_string(cpu_running_time_sec); }

}; // struct Sort_stats

// … “`

For this assignment, num_comparisons is the number of times &lt; or &lt;= is called on the values in the vector. It has the type ulong (unsigned long) because the comparison counts can get very large.

You should modify the code of the sorting functions to return accurate Sort_stats objects. You can write helper functions if you like.

Example: Bubble Sort

For example, you can implement bubble sort like this:

“`cpp template Sort_stats bubble_sort(vector &amp;v) { ulong num_comps = 0; // &lt;— num_comps is initialized to 0 here clock_t start = clock();

for (int i = 0; i &lt; v.size(); i++)

{

for (int j = 0; j &lt; v.size() – 1; j++)

{

num_comps++; // &lt;— num_comps is incremented here if (v[j] &gt; v[j + 1])

{

T temp = v[j]; v[j] = v[j + 1]; v[j + 1] = temp;

}

} }

clock_t end = clock(); double elapsed_cpu_time_sec = double(end – start) / CLOCKS_PER_SEC;

return Sort_stats{“Bubble sort”,

v.size(), num_comps, elapsed_cpu_time_sec};

} “`

Timing Code in C++

As shown in bubble_sort, CPU time can be measured using clock() like this:

“`cpp

include

void timed_experiment() { clock_t start = clock();

//

// … do stuff …

// clock_t end = clock(); double elapsed_cpu_time_sec = double(end – start) / CLOCKS_PER_SEC; cout &lt;&lt; “It took ” &lt;&lt; elapsed_cpu_time_sec &lt;&lt; ” seconds to do stuff. “;

} “` cpu_timer_example.cpp contains an example of timing code.

Helper Functions

In addition to the sorting routines, there are two other helper functions in a4_base.h that you need to implement:

is_sorted(v) returns true if the vector is sorted in ascending order, and false otherwise. Its worst-case running time should be linear in the size of v.

rand_vec(size, min, max) returns a vector of size random integers, where the integers range from min to max (both min and max are included). Its worst-case running time should be linear in size.

Both of these functions are helpful when testing sorting routines, so you should implement them first.

Generating the Experimental Data

When your sorting algorithms are ready, use them to generate the following data:

For each of the 8 sorting algorithms, do the following:

For N = 2000, 4000, 6000, …, 50000 (25 different values of N) do the following:

create a vector of N random integers, where the numbers in the vectors range from 1 to N run the sort on the vector of random integers print the sort name, amount of data being sorted, number of comparisons that were done, and the CPU time (in seconds)

Since there are 8 algorithms and 25 values of N, you’ll end up with 8 * 25 = 200 results.

If you print the individual results as comma separated values (CSVs), then you can more easily import them into a spreadsheet. For example, here are 4 calls to bubble sort printed as comma separated values:

Bubble sort, 2000, 3998000, 0.003197 Bubble sort, 4000, 15996000, 0.014169 Bubble sort, 6000, 35994000,

0.035031 Bubble sort, 8000, 63992000, 0.066863

If you save this output in a file, the file should be readable by Excel or Google Sheets as a CSV file.

Visualizing the Data in a Spreadsheet

Using Excel or Google Sheets, create a table of all the data you generated. Here us an example of what the first four rows of the table ought to look like (the exact numbers in your table might be different):

| Name | N | Comparisons | CPU Seconds | |————-|——-|—————–|—————–| | bubble sort | 2000 | 3998000 | 0.003197 | | bubble sort | 4000 | 15996000 | 0.014169 | | bubble sort | 6000 | 35994000 | 0.035031 | | bubble sort | 8000 | 63992000 | 0.066863 | The table should have 4 columns, and each column is labelled with the given name, as shown.

Remember The table will have 200 rows of data.

In addition to this table, draw four line graphs, where the x-axis of each graph is N (the size of the vector being sorted), and has the values from the data you generated: N=2000, 4000, 6000, …, 50000. The four graphs are:

Graph 1: CPU time for bubble sort, insertion sort, selection sort, and shell* sort. The the y-axis is the CPU time in seconds.

Graph 2: CPU time for merge sort, quick sort, iquick sort, and priority queue sort. The y-axis is the CPU time in seconds.

Graph 3: comparison counts for bubble sort, insertion sort, selection sort, and shell sort. The y-axis is the number of comparisons.

Graph 4: comparison counts for merge sort, quick sort, iquick sort, and priority queue sort. The y-axis is the number of comparisons.

Each graph will have 4 lines on it, one for each of the sorting algorithms it is plotting data for.

Make these graphs beautiful and easy to read. Give them descriptive titles (don’t just name them Graph 1, Graph 2, etc.!), clearly labelled x and y axes, and use colors or textures to distinguish different lines on the same graph.

Note It’s not too hard to make nice-looking graphs in Excel or Google Sheets. Spend a bit of time playing with the options.

What to Submit

When you’re done, submit a zip file containing just these two files:

a4_sort_implementations.h

An Excel or Google Sheets file named a4.xlsx that contains the table of experimental data and the 4 graphs.

Grading

The marker will compile and run your program on Ubuntu Linux using makefile like this:

“`bash

make a4_test g++ -O3 -std=c++17 -Wall -Wextra -Werror -Wfatal-errors -Wno-sign-compare -Wnon-virtual-dtor -g a4_test.cpp

-o a4_test

./a4_test … testing output …

valgrind ./a4_test … valgrind output … “`

The file a4_test.cpp is a test program written by the marker that tests the correctness of your sorting algorithms (it is not provided here!). It will include a4_base.h and

a4_sort_implementations.h.

Note that the -O3 flag is one of the options: this asks g++ to optimize the code for speed.

Note The compilation commands are quite strict! Make sure your program compiles with them before submitting it.

Marking Scheme

1 mark for a correct and efficient implementation of is_sorted(v)

1 mark for a correct and rand_vec(size, min, max).

All code is sensibly and consistently indented, and all lines are 100 characters in length, or less.

Whitespace is used to group related pieces of a code to make it easier for humans to read. All whitespace has a purpose.

Variable and function names are self-descriptive.

Appropriate features of C++ are used, as discussed in class and in the notes. Note If you use a feature that we haven’t discussed in class, you must explain it in a comment, even if you think it’s obvious.

Comments are used when needed to explain code whose purpose is not obvious from the code itself. There should be no commented-out code from previous versions.

`### Deductions

you don’t include the “Statement of Originality”, or it is modified in any way
