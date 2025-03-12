# heap-benchmarks
A heap data structure benchmark dataset.

Record structure <id, priority, operation type>.

Operation type: 0 deletes the element with the lowest priority; 1 inserts an element; 2 increases the priority; 3 decreases the priority;


Fibonacci heap, d-ary heap, binomial heap and skew heap in boost lib crash on multiple datasets including mix_25.edges!
Pairing heap crashes on larger datasets too!
https://github.com/boostorg/boost/issues/1017

d-ary heap:
   void increase(size_type index)
    {
      siftdown(index);//siftup(index);
    }
    void decrease(size_type index)
    {
      siftup(index);//siftdown(index);
    }
