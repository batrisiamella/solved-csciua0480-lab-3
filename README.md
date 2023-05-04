Download Link: https://assignmentchef.com/product/solved-csciua0480-lab-3
<br>
Before you start:

<ul>

 <li>To calculate the time of each program in this lab use the Linux command time.</li>

 <li>After you login to your CIMS account, you need to ssh to one of the following: cuda1, cuda2, cuda3, or cuda4</li>

 <li>The source code, containing both device and host code, has extension .cu</li>

 <li>You compile with <strong>nvcc</strong>cu</li>

 <li>Don’t forget to #include &lt;cuda.h&gt;</li>

 <li>A very useful API is <strong>cudaGetDeviceProperties</strong>() check it up.</li>

</ul>

<strong> </strong>

<ol>

 <li>Assume a reduction algorithm that finds the maximum of an array of 8192 integers. You will need to write a host function that fills the array with random integers between 1 and 100000.

  <ol start="8192">

   <li>Write the sequential version of the program in C. Note that the sequential version will scan the array sequentially from start to end. Call it <strong>c</strong>.</li>

   <li>Write a CUDA version of the program that does not take thread divergence into account. Call it <strong>cu</strong>.</li>

   <li>Update the version in B to take thread divergence into account. Call it <strong>cu</strong>.</li>

   <li>Update the program in C to make use of shared memory to reduce global memory bandwidth. Call it <strong>cu</strong>.</li>

  </ol></li>

</ol>

Draw a bar graph that compares the execution time of each of the above 4 versions. That is, x-axis contains the 4 versions (for each one report the real, user, and sys) and the y-axis contains the time. So, we expect to see 12 bars (4 versions and 3 timing each).




<ol start="2">

 <li>Repeat problem 1 with an array of 65536 elements. Adjust the file names based on the new number.</li>

</ol>




<ol start="3">

 <li>What can we conclude from the results of problems 1 and 2 regarding the optimizations and the problem size?</li>

</ol>