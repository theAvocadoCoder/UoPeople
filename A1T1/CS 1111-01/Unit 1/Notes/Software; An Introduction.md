## Introduction
There are 2 software categories
- ==System Software==: Responsible for the coordination of all activities in a computer system.
- ==Application Software==: Written with a specific purpose in mind. Allows users work in English or give commands in a  format not dependent on computer hardware. It is divided into general purpose apps and tailor-made apps.
## Operating System
This is system software. It coordinates the flow of information from the computer to the user and vice versa.
### Functions of the OS
- **Memory Management**: Loads programs from RAM to hard disk & frees up RAM after execution.
- **CPU Management**: Handles job scheduling for the microprocessor. Processor gets job from memory, processes the job, passes it on and gets ready for the next job.
- **Disk Management**
- **Input/Output Management**: Device drivers ( or support utility programs of the OS) are supporting software required by the system to make input and output devices work properly. They are controlled by the OS.
- **User Interface**: OS provides a command interpreter to bridge the gap between human and machine language.
- **Communication**: OS facilitates information exchange between processes running on a computer system. Communication is either via shared memory or 'message passing' (i.e., the OS moving packets of information between processes).
- **Error Detection**: OS keeps track of all possible errors and prompts the erring user via an appropriate message on the computer screen.
- **Resource Allocation**: Processing time, RAM, storage, devices, etc. must be allocated to all users equally by the OS.
- **Accounting**: Comprehensive record-keeping of computer resources used by a user. Useful for improving computing services.
- **Protection**: OS provides a multilevel mechanism for data protection achieved via access control to system resources. This includes an authentication process by means of multilevel password protection system. Provided by an OS.
### Types & Classifications of Operating Systems
- ==Batch Processing System Software==: Jobs are processed on a FIFO basis. Memory is divided into 2 parts: one is permanently occupied by the software; the other is used as per the need of the user. Instructions are executed in batches, saving processor time.
- ==Multi-User Operating System Software==: Multiple terminals (inits of PCs) are attached to the main computer system as in minicomputers and mainframe systems. One CPU (microprocessor) to perform all operations. e.g. UNIX, MSV.
- ==Multi-programming or Multitasking System Software==: These are capable of running more than one program ata  time. Multi-programming is the process of creating a situation in which more than one program may be held in the main memory at one time. The purpose is to minimize unused microprocessor time. Rapid nob switching under time-sharing mode. Goes through jobs sequentially in time slices over and over. Processor is kept busy while channels and buffers bring data and write out information. e. g. UNIX, OS/3, Windows.
- ==Multi-processing Operating System Software==: It uses multiple processor that share a common memory. Instructions from different and independent programs processed at the same rime or instructions from the same program executed simultaneously, e.g. UNIX OS/2 MSV. There are for types of this OS:
	- Loosely coupled multi-processing
	- Functional specialized processors
	- Tightly coupled multi-processors
	- Parallel processing
	Often, 2 or more processors, each with its own control unit, ALU, etc, allowed to access shared main memory and input/output devices, can communicate through memory or directly exchange signals. OS controls all, facilitates interactions between the processor(s) and program.
- ==Real-Time System Software==: Response time is critical. Involved with the immediate processing of data, machines and records. Designed to accept data in real time. They are online systems with tighter constraints on response time. e.g. C Executive, communications control program (CCP), CTOS, CTRON, FADOS, etc.
### Components of an Operating System
There are two primary components, viz: a supervisor; and an integrated set of support utilities.
- **Supervisor** (or Control Program): A set of inter-integrated programs that takes care of the overall working of the computer system. It has 3 basic functions (in addition to keeping track of time):
	- Initializes system at startup.
	- Allows running of application programs.
	- Controls IO devices attached to the system.
	The OS is generally found on the hard disk and sometimes in the form of a chip called firmware. The supervisor has 2 portions: a kernel and a transient portion. When the supervisor is first loaded into memory, both portions are loaded. The kernel always stays in memory to monitor system operations. Since it interacts directly with hardware, it must be present in memory as long as the computer is in use.
- **The Support Utilities**: These are classified into 3, viz;
	- _Program Development Utilities_ e.g. assemblers, editors, interpreters, compilers, and linkers.
	- _System Management Utilities_ e.g. programs that keep track of more than 1 user, diagnostic routines, etc.
	- _File Management Utilities_ e.g. programs for copying files, erasing, printing, renaming, etc.