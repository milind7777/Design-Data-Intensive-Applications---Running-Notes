<h2> Reliable, Scalable, and Maintainable Applications </h2>

1. **Reliability** - A system should continue to perform *correctly*(performing the correct function at desired level of performance) even in the face of *adversity*(hardware or software faults, human error).

* Hardware faults - Causes - Hard disks crash, RAM becomes faulty, the power grid has a blackout, someone unplugs the wrong network cable.

* Simple fixes - Add redundancy to individual hardware components - 
    * Organise disks in a [RAID(Redundant Array Independent Disks)](https://www.techtarget.com/searchstorage/definition/RAID#:~:text=RAID%20(redundant%20array%20of%20independent%20disks)%20is%20a%20way%20of,case%20of%20a%20drive%20failure.) configurations - Does data mirroring(having multiple copies of data across drives) and data striping(partitioning single data along multiple drives to improve read performance) to achieve redendancy and performance.
    * Server can have dual power supplies and [hot-swappable](https://en.wikipedia.org/wiki/Hot_swapping) CPUs.
    * Data centers may be batteries and diesel generators for back power.

* Hardware component redundancy makes total failure of single machine rare. But current data intensive systems use a large number of machines, increasing the rate of failures, hence there is move towards systems that can tolerate multiple machine failures, by using software fault tolerance techniques.

* Software faults - examples - Bug that causes every instance of an application server to crash, a runaway process that uses up shared CPU, a service that the system depends on slows down, or becomes completely unresponsive, a software bug that introduces cascading failures.

* No easy solutions - extensive testing under crash scenarios.

2. Scalability

* Potential load parameters - 