[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/9YUeXH71)
# Theoretical Sorting

A Computer Science researcher claims to have come up with a sorting algorithm
that can sort arbitrary elements in $O(n)$ time based on comparisons of two
elements at a time. This would be asymptotically faster than any known general
sorting algorithm. The algorithm itself is proprietary and will be sold by a
company.

How would you verify this claim? You may assume that you have access to a
black-box implementation of the sorting algorithm, i.e. you cannot examine the
source code, but you can use it to sort any list you like. Explain in detail
your method for investigating whether X is correct, including any expected
results you would get.

Also give a theoretical argument for why X could or could not be correct, based
on the complexity of the general sorting problem we covered in class.

Add your answers to this markdown file.

Answer:

To verify this claim, I would start with analyzing the algorithms runtime with small and large input sizes. Assuming the runtime of the algorithm is $O(n)$, the runtime should linearly grow as the input size increases. If the runtime is consistantly increasing as I run it with larger and larger input sizes, it would prove that the claim that the algorithm's runtime of $O(n)$ might actually be accurate.

I would then start analyzing the algorithms runtime with special and unique inputs such as completely random data sets and data sets that contain repeated elements. If the runtime of these unique datasets, depending on their size, are consistent with the runtimes of the datasets that are consistently increasing (as mentioned above), then it would also further help the claim's credibility.

I could also begin to compare the algorithms performance to other well known sorting algorithms. If the algorithm sorts a given dataset faster than quicksort or mergesort ( $O(n log n)$ ), then it would also prove that the claim could be accurate.

If all of the previously suggested tests pass then this new sorting algorithm would truly have a revolutionary runtime of $O(n)$. In reality, this could not be true because according to the slides and Stirling's approximation, any comparison-based sorting algorithm can not surpass a runtime of $O(n log n)$.
