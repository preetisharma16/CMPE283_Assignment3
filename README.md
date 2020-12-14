
#  CMPE283 : Virtualization Technology
   CMPE283_Assignment3:  Instrumentation via hypercall
   
   Student names: Priti Sharma(014561274)
   
   University Name: San Jose State University
   
   
   Prerequisites:
   
   You will need a machine capable of running Linux, with VMX or SVM virtualization features exposed. 
   You may be able to do this inside a VM, or maybe not, depending on your hardware and software configuration. 
   Using the environment setup created for assignment 2.
  
# Question 1: 
   Its an individual assignment. Completed by Priti Sharma(014561274)
   
# Question 2:

   Steps required for this Assignment:
   
   1. Running this assignment on Linux machine(400 GB hard disk space and 15 GB memory) with SVM virtualization features exposed
     and has AMD processor.
     run $ cat/proc/cpuinfo | more
     
   ![image 1](./pic/cpuinfo.png?raw=true )
     
   2. verify processor support for KVM, output should be “kvm-ok” and “KVM acceleration can be used”.
   
   ![image 1](./pic/kvminfo.png?raw=true )
   
   3. Modified vmx.c and cpuid.c program files.
   
   4. build it make && make modules && make install && make modules_install 
   
   5. Open Terminal in the inner VM and call cpuid code with cpuid -l 0x4ffffffe



