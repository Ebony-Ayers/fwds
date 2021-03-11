# FWDS (Fast Wasteful Data Structures)
Does what it says on the tin. A set of data structures designed to be as fast as possible at the cost of memory wastage.
All data structures are provided in thread safe and thread unsefe versions.

Data structure | type name | Description | Time complexity | Memory notes
------------ | ------------- | ------------- | ------------- | -------------
Queue | queue | Simple FIFO queue | enqueue O(1), dequeue O(1) | Data is garanteed continguous and the control block will be near the data but not garanteed next to it
Small int priority queue | sipqueue | Priority queue with p integer discrete priorities set at compile-time | enqueue O(1), dequeue O(1) | The data is garanteed to be in one block flowing the control block but the data will NOT be in order
Stack | stack | simple stack | push O(1), pop O(1) | Data is garanteed contiguous and will be following the control block
Run-time array | rd_array | non expandable run-time dynimic array | get O(1), set O(1) | Data is garanteed contigous
Compile-time dynamic array | cd_array | non expandable compile-time dynimic array | get O(1), set O(1) | Data is garanteed contigous
Compile-time static array | cs_array | non expandable compile-time static array | get O(1), set O(1) | Data is garanteed contigous
List | list | expandable list, equivilent to std::vector | get O(1), set O(1), append O(1), insert O(n) | Data is garanteed contigous
Singily linked list |sllist | singily linked list | get O(1), set O(1), insert O(1), random get O(n), random set O(n), random insert O(n) | Data is in one block but NOT in order
