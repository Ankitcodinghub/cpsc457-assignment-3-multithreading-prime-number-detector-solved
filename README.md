# cpsc457-assignment-3-multithreading-prime-number-detector-solved
**TO GET THIS SOLUTION VISIT:** [CPSC457 Assignment 3-Multithreading-Prime-Number-Detector Solved](https://www.ankitcodinghub.com/product/cpsc457-assignment-3-multithreading-prime-number-detector-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;92167&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CPSC457 Assignment 3-Multithreading-Prime-Number-Detector Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
Q1. Programming question – calculating 𝛑

Improve the performance of an existing single-threaded calcpi program by converting it to a

multi-threaded implementation. Download the starter code, compile it, and run it:

The calcpi program estimates the value of π using an algorithm described in https://en.wikipedia.org/wiki/Approximations_of_%CF%80#Summing_a_circle’s_area, and it is implemented inside the function count_pi() in file calcpi.cpp.

The included driver (main.cpp) parses the command line arguments, calls count_pi() and prints the results. The driver takes 2 command line arguments: an integer radius and number of threads. For example, to estimate the value of π using radius of 10 and 2 threads, you would run it like this:

The function uint64_t count_pi(int r, int N) takes two parameters – the radius and number of threads, and returns the number of pixels inside the circle or radius 𝑟 centered at (0,0) for every pixel (𝑥, 𝑦) in squre −𝑟 ≤ 𝑥, 𝑦 ≤ 𝑟. The current implementation is single threaded, so it ignores the N argument. Your job is to re-implement the function so that it uses N threads to speed up its execution, such that it runs N times faster with N threads on hardware where N threads can run concurrently. Please note that your assignment will be marked both for correctness and the speedup it achieves.

You need to find a way to parallelize the algorithm without using any synchronization mechanisms, such as mutexes, semaphores, atomic types, etc. You are only allowed to create and join threads.

Write all code into calcpi.cpp and submit this file for grading. Make sure your calcpi.cpp works with the included driver program. Your TAs may use a different driver program during

</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
<pre>$ git clone https://gitlab.com/cpsc457f21/pi-calc.git
$ cd pi-calc
$ make
$ ./calcpi
</pre>
<pre>Usage: ./calcpi radius n_threads
   where 0 &lt;= radius &lt;= 100000
     and 1 &lt;= n_threads &lt;= 256
</pre>
</div>
</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
<pre>$ ./calcpi 10 2
Calculating PI with r=10 and n_threads=2
count: 317
PI:    3.17</pre>
</div>
</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="section">
<div class="layoutArea">
<div class="column">
marking, so it is important that your code follows the correct API. Make sure your program runs on linuxlab.cpsc.ucalgary.ca.

Assume 0 ≤ 𝑟 ≤ 100,000 and 1 ≤ 𝑛𝑡h𝑟𝑒𝑎𝑑𝑠 ≤ 256. Timing on linuxlab

Please note that not all linuxlab machines are the same. Some have 4 core CPUs, some have 6 cores CPUs, some have 3.6GHz CPUs, others have 3.2GHz. You can check which CPU you have by running lscpu command. When you are running your timings, please make sure you do all of them on the same machine. Otherwise, you will get very inconsistent results.

My basic multi-threaded implementation achieves the following timings using r=100000. I expect your solutions to achieve similar results.

</div>
</div>
<div class="layoutArea">
<div class="column">
CPU 1 thread 2 threads 4 threads

i7-4770 12.900 6.470 3.410 i7-4790 12.571 6.306 3.311 i7-7700 11.473 5.857 3.006 i7-8700 10.476 5.374 2.793

Q2 – Written answer [3 marks]

</div>
<div class="column">
8 threads 16 threads

2.733 2.740 2.653 2.688 1.765 1.801 1.610 1.161

</div>
</div>
<div class="layoutArea">
<div class="column">
Time your multi-threaded solution from Q1 with 𝑟 = 50000 using the time command on linuxlab.cpsc.ucalgary.ca. Record the real-time for 1, 2, 3, 4, 6, 8, 12, 16, 24 and 32 threads. Also record the timings of the original single-threaded program.

A. Make a table with these timings, and a bar graph, both formatted similar to these:

</div>
</div>
<table>
<tbody>
<tr>
<td>
<table>
<tbody>
<tr>
<td>
<div class="layoutArea">
<div class="column">
Threads

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
Timing (s)

</div>
</div>
</td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
1 (original)

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
5

</div>
</div>
</td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
1

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
4

</div>
</div>
</td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
2

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
8

</div>
</div>
</td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
3

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
7

</div>
</div>
</td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
4

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
3

</div>
</div>
</td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
6

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
2

</div>
</div>
</td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
8

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
11

</div>
</div>
</td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
12

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
15

</div>
</div>
</td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
16

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
7

</div>
</div>
</td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
24

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
2

</div>
</div>
</td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
32

</div>
</div>
</td>
<td>
<div class="layoutArea">
<div class="column">
14

</div>
</div>
</td>
</tr>
</tbody>
</table>
</td>
</tr>
<tr>
<td>
<div class="layoutArea">
<div class="column">
The numbers in the above table and graph are random. Your timings should look different.

</div>
</div>
</td>
</tr>
</tbody>
</table>
<div class="layoutArea">
<div class="column">
<ol start="2">
<li>When you run your implementation with N threads, you should see N-times speed up compared to the original single threaded program. Do you observe this in your timings for all values of N?</li>
<li>Why do you stop seeing the speed up after some value of N?</li>
</ol>
</div>
</div>
<div class="layoutArea">
<div class="column">
CPSC 457: Assignment 3 2

</div>
</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="layoutArea">
<div class="column">
Q3. Programming question – detecting primes [30 marks]

Convert a single-threaded program detectPrimes to a multi-threaded implementation. Start by downloading the single-threaded code, then compile it and run it:

</div>
</div>
<div class="section">
<div class="layoutArea">
<div class="column">
<pre>$ git clone https://gitlab.com/cpsc457f21/detect-primes.git
$ cd detect-primes
$ make
$ cat example.txt
</pre>
0 3 1925 4012009 165 1033

<pre>$ ./detectPrimes 5 &lt; example.txt
Using 5 threads.
Identified 3 primes:
</pre>
<pre>  3 19 1033
Finished in 0.0000s
</pre>
<pre>$ seq 100000000000000000 100000000000000300 | ./detectPrimes 2
Using 2 threads.
Identified 9 primes:
</pre>
100000000000000003 100000000000000013 100000000000000019 100000000000000021 100000000000000049 100000000000000081 100000000000000099 100000000000000141 100000000000000181

<pre>Finished in 5.6863s
</pre>
</div>
</div>
</div>
<div class="layoutArea">
<div class="column">
The detectPrimes program reads integers in range [2, 263 − 2] from standard input, and then prints out the ones that are prime numbers. The first invocation example above detects prime numbers 3, 19 and 1033 in a file example.txt. The second invocation uses the program to find all primes in the range [1017, 1017 + 300]. If duplicate primes appear in the input, they will be duplicated in the output.

detectPrimes accepts a single command line argument – a number of threads. This parameter is ignored in the current implementation because it is single threaded. Your job is to improve the execution time of detectPrimes by making it multi-threaded, and your implementation should use the number of threads given on the command line. To do this, you will need to re-implement the function:

which is defined in detectPrimes.cpp. The function takes two parameters: the list of numbers to test, and the number of threads to use. The function is called by the driver (main.cpp) after parsing the standard input and command line. Your implementation should use n_threads number of threads. Ideally, if the original single-threaded program takes time 𝑇 to complete a test, then your multi-threaded implementation should finish that same test in 𝑇/𝑁 time when using 𝑁 threads. For example, if it takes 10 seconds to complete a test for the original single- threaded program, then it should take your multi-threaded program only 2.5 seconds to complete that same test with 4 threads. To achieve this goal, you will need to design your program so that:

• You give each thread the same amount of work;

CPSC 457: Assignment 3 3

</div>
</div>
<div class="layoutArea">
<div class="column">
<pre>std::vector&lt;int64_t&gt;
detect_primes(const std::vector&lt;int64_t&gt; &amp; nums, int n_threads);
</pre>
</div>
</div>
</div>
<div class="page" title="Page 4">
<div class="layoutArea">
<div class="column">
<ul>
<li>your multi-threaded implementation does the same amount of work as the single-threaded version; and</li>
<li>the synchronization mechanisms you utilize are efficient.
Your TAs will mark your assignment by running the code against multiple different inputs and using different numbers of threads. To get full marks for this assignment, your program needs to output correct results but also achieve near optimal speedup for the given number of threads and available cores. If your code does not achieve optimal speedup on all inputs, you will lose some marks for those tests.

You may assume that there will be no more than 100,000 numbers in the input, and that all numbers will be in the range [2, 263 − 2]. Some inputs will include many numbers, some inputs will include just few numbers, some numbers will be large, some small, some will be prime numbers, others will be large composite numbers, etc… For some numbers it will take long time to compute their smallest factor, for others it will take very little time. You need to take all these possibilities into consideration. Design your own test inputs and test your code thoroughly.

Write all code into detectPrimes.cpp and submit it for grading. Make sure your detectPrimes.cpp works with the included main.cpp driver. We may use a different driver during marking, so it is important that your code follows the correct API. Make sure your program runs on linuxlab.cpsc.ucalgary.ca.

You may use any of the synchronization mechanisms we covered in lectures, such as semaphores, mutexes, condition variables, spinlocks, atomic variables, and barriers. Don’t forget to make sure your code compiles and runs on linuxlab.cpsc.ucalgary.ca.

Please note that the purpose of this question is NOT to find a more efficient factorization algorithm. You must implement the exact same factorization algorithm as given in the skeleton code, except you need to make it multi-threaded.

Q4 – Written question (5 marks)

Time the original single-threaded detectPrimes.cpp as well as your multi-threaded version on three files: medium.txt, hard.txt and hard2.txt. For each of these files, you will run your solution 6 times, using 1, 2, 3, 4, 8 and 16 threads. You will record your results in 3 tables, one for each file, formatted like this:
</li>
</ul>
</div>
</div>
<div class="layoutArea">
<div class="column">
# threads

original program 1

2

3

4

8

16

</div>
<div class="column">
Observed timing

</div>
<div class="column">
medium.txt

Observed speedup compared to original

1.0

</div>
<div class="column">
Expected speedup

1.0 1.0 2.0 3.0 4.0 8.0 16.0

</div>
</div>
<div class="layoutArea">
<div class="column">
CPSC 457: Assignment 3

</div>
<div class="column">
4

</div>
</div>
</div>
<div class="page" title="Page 5">
<div class="layoutArea">
<div class="column">
The ‘Observed timing’ column will contain the raw timing results of your runs. The ‘Observed speedup’ column will be calculated as a ratio of your raw timing with respect to the timing of the original single-threaded program. Once you have created the tables, explain the results you obtained. Are the timings what you expected them to be? If not, explain why they differ.

Submission

Submit the following files to D2L for this assignment.

Do not submit a ZIP file. Submit individual files.

</div>
</div>
<div class="layoutArea">
<div class="column">
calcpi.cpp detectPrimes.cpp report.pdf

</div>
<div class="column">
solution to Q1

solution to Q3

answers to all written questions

</div>
</div>
<div class="layoutArea">
<div class="column">
Please note – you need to submit all files every time you make a submission, as the previous submission will be overwritten.

</div>
</div>
</div>
<div class="page" title="Page 6">
<div class="layoutArea">
<div class="column">
&nbsp;

</div>
</div>
</div>
<div class="page" title="Page 7">
<div class="layoutArea">
<div class="column">
Hint 3 –good solution

Even more efficient approach would be to parallelize the inner loop (the loop inside the is_prime function). In this approach, all threads would test the same number for primality. If you choose this approach, you need to give each thread a different portion of divisors to check. This will allow you to handle more input cases than the simple solution mentioned earlier. For extra efficiency, and better marks, you also need to consider implementing thread re-use, e.g., by using barriers. Here is a possible rough outline of an algorithm that you could implement:

detectPrimes():

prepare memory for each thread

initialize empty array result[] – this could be a global variable set global_finished = false – make it atomic to be safe

start N threads, each runs thread_function() on its own memory join N threads

return results

<pre>thread_function():
  repeat forever:
</pre>
<pre>    serial task – pick one thread using barrier
      get the next number from nums[]
      if no more numbers left:
</pre>
<pre>        set global_finished=true to indicate to all threads to quit
      otherwise:
</pre>
<pre>        divide work for each thread
    parallel task – executed by all threads, via barrier
</pre>
<pre>      if global_finished flag is set, exit thread
</pre>
<pre>      otherwise do the work assigned above and record per-thread result
    serial task – pick one thread using barrier
</pre>
<pre>      combine the per-thread results and update the result[] array if necessary
</pre>
You may use my C++ barrier implementation from lecture notes.

Hint 4 – best solution

This builds on top of the hint 3 above, but it also adds thread cancellation. You need cancellation for cases where one of the threads discovers the number being tested is not a prime, so that it can cancel the work of the other threads. Thread cancellation sounds simple to implement, but it does take non-trivial effort to get it working correctly.

Appendix – Approximate grading scheme for Q3

The test cases that we will use for marking will be designed so that you will get full marks only if you implement the most optimal solution. However, you will receive partial marks even if you one of the less optimal solutions. Here is the rough breakdown of what to expect depending on which solution you implement:

<ul>
<li>Parallelization of outer loop with fixed amount of work will yield ~9/28 marks</li>
<li>Parallelization of outer loop with dynamic work will yield ~15/28 marks</li>
<li>Parallelization of inner loop without work cancellation and without thread reuse will yield
~19/28 marks
</li>
</ul>
</div>
</div>
<div class="layoutArea"></div>
</div>
<div class="page" title="Page 8">
<div class="layoutArea">
<div class="column">
<ul>
<li>Parallelization of inner loop with thread reuse but without cancellation will yield ~24/28 marks.</li>
<li>Parallelization of inner loop with thread reuse and with cancellation will give 28/28 marks.
Any tests on which your program produces wrong results will receive 0 marks.
</li>
</ul>
</div>
</div>
</div>
