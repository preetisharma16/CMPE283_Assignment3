#  CMPE283 : Virtualization Technology
   
   CMPE283_Assignment4: Nested Paging vs. Shadow Paging
   
   Student names: Priti Sharma(014561274)
   
   University Name: San Jose State University
   
   
   Prerequisites:
   
   A working assignment 3.
  
# Question 1: 
   Its an individual assignment. Completed by Priti Sharma(014561274)
   
# Question 2:
  Steps performed :
  
  1. Below is the output of total number of exit count after completing assignment 3 and before removing the kernel modules.
  
  ![image 1](./pics/out1.png?raw=true )
  
  2. Remove kernel modules and verfify kernels are removed properly 
  
  ![image 1](./pics/out2.png?raw=true )
  
  
  3. Now inserting kernels with ept=0 with command insmod /lib/modules/XXX/kernel/arch/x86/kvm/kvm-intel.ko ept=0. 
     where XXX is the version of the kernel you build for assignment 3.
     
 ![image 1](./pics/out3.png?raw=true )
  
  4. check total number of exits after rebooting
  
  ![image 1](./pics/out4.png?raw=true )
  
  
# Question 3: 
  What did you learn from the count of exits? Was the count what you expected? If not, why not? 
  
  Answer: Total number of exit count increased when kernel is running with ept value "0". 
          This is expected because here we are enforcing shadow paging by loading the kernel module with ept=0 value.

# Question 4:
  What changed between the two runs (ept vs no-ept)?
  
  Answer: This assignment shows how to enforce shadow paging With ept, thus results in increased total number of exits.
          with no-ept total number of exits did not increase rapidly as contrast to shadow paging.

