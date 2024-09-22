# Cloud Computing

<img width="900px" src="./assets/logosImages/cloudComputingImage.jpg" alt="Cloud Computing Image">

### Virtualization

Virtualization is a technology that allows a single physical computer or server to be divided into multiple virtual machines, or "VMs". These VMs can then run different operating systems or applications while sharing the resources of the host machine.

Virtualization can help businesses use their hardware more efficiently, and can also power cloud computing services. Some benefits of virtualization include: 
- **Improved scalability**: Virtualization can help improve scalability and workloads. 
- **Reduced infrastructure costs**: Virtualization can result in the use of fewer servers, which can reduce infrastructure costs and maintenance. 
- **Reduced energy consumption**: Virtualization can help reduce energy consumption. 
- **Access to a larger app library**: Enabling virtualization on a Windows device can give you access to a larger library of apps.

There are several different types of virtualization, including: 
- **Desktop virtualization**: Allows a centralized server to manage and deliver individualized desktops. 
- **Network virtualization**: Splits network bandwidth into independent channels that can be assigned to specific devices or servers. 
- **Software virtualization**: Separates applications from the operating system and hardware. 
- **Data virtualization**: Allows companies to manage data by bringing together data from multiple sources. 

---

### Hypervisor

A hypervisor is a software, firmware, or hardware component that allows a single physical machine to run multiple virtual machines (VMs):

|  |  |
| :--: | :-- |
|  What it does  |  Allocates a physical machine's resources, such as memory and CPU, to individual VMs  |
| Other names | Virtual machine monitor (VMM), virtualizer |
| How it works | Acts as a supervisor that distributes the components that make up VMs |
| Benefits | Makes it easier and more cost-effective to clone and replicate VMs |
| Uses | Test environments, desktop virtualization, industrial control automation consolidation |
| Vulnerability | A target for hackers, especially those coming from a rogue VM |
| | |

The physical machine that runs a hypervisor is called the host machine, and each VM is called a guest machine.

There are two main types of hypervisors: **Type 1** and T**ype 2**:

**Type 1**
*Also known as a bare metal or native hypervisor, this type of hypervisor runs directly on the host's hardware. It's often used in data centers, web servers, and other server-based environments. Type 1 hypervisors are generally more secure and stable than Type 2 hypervisors because they don't run on top of another operating system.* 

**Type 2**
*Also known as a hosted hypervisor, this type of hypervisor runs as a software layer on top of an operating system. It's often used in desktop and development environments. Type 2 hypervisors are easier to install, configure, and use than Type 1 hypervisors.* 

Both *Type 1* and *Type 2* hypervisors use hardware acceleration support, but to different degrees. *Type 1* hypervisors typically don't function without hardware acceleration technologies, while *Type 2* hypervisors can usually fall back on software emulation if hardware acceleration isn't available. 

    Hardware acceleration is the process of using specialized hardware components to perform tasks more efficiently than software running on a general-purpose processor. It can improve performance and reduce the load on the CPU.

**Type 1** and **Type 2** hypervisors differ in several ways, including: 

**Performance**
*Type 1 hypervisors are generally faster and more efficient than Type 2 hypervisors because they have direct access to the host computer's hardware, while Type 2 hypervisors must operate through the operating system.*

**Resource allocation**
*Type 1 hypervisors can implement their own resource allocation strategies, while Type 2 hypervisors must negotiate with the operating system.*

**Ease of management**
*Type 1 hypervisors are more complex and require system administrator-level knowledge to manage, while Type 2 hypervisors can be installed and managed like an application on an operating system.* 

**Hardware requirements**
*Type 1 hypervisors require dedicated hardware with ample resources, while Type 2 hypervisors can operate on standard desktops or laptops.* 

**Use cases**
*Type 1 hypervisors are more common in large data centers and enterprise-level computing workloads, while Type 2 hypervisors are more commonly used for non-resource-intensive workloads and in environments with a small number of servers.* 

When choosing a hypervisor, it's important to consider the specific needs of the organization or deployment, such as performance, scalability, security, and management capabilities. 

---

### VMware Workstation

<img width="400px" src="./assets/logosImages//vmwarelogo.png" alt="VMware Logo">

VMware Workstation is a desktop virtualization product that allows users to run multiple operating systems on the same computer without rebooting.

VMware Workstation Pro is a hosted hypervisor that runs on x64 versions of Windows and Linux operating systems. There used to be an IA-32 version for earlier versions for the software. It enables users to set up virtual machines on a single physical machine and use them simultaneously along with the host machine.

VMware Workstation allows users to: 

**Create virtual machines**
*Users can create virtual machines that replicate server, desktop, and tablet environments.* 

**Allocate resources**
*Users can allocate resources like processor cores, memory, and graphics memory to each virtual machine.* 

**Develop and test software**
*Users can develop, test, and demonstrate software by running multiple operating systems simultaneously.* 

**Learn about technology**
*Users can build and test software, browsers, apps, and games.*

*VMware Workstation is available for Windows, Linux, and Mac computers. As of May 13, 2024, VMware Workstation Pro will be free for personal use, but commercial use will still require a license.*

---

### VirtualBox

<img width="400px" src="./assets/logosImages//virtualboxlogo.png" alt="VirtualBox Logo">

Oracle VirtualBox is a hosted hypervisor for x86 virtualization developed by Oracle Corporation. As an open-source virtualization platform with built-in support for guest operating system functionality, Oracle VirtualBox is freely available for personal and commercial use, enabling users to run virtual machines without complex configuration or hardware changes.

---

### Windows Sandbox

<img width="400px" src="./assets/logosImages//windowsSandbox.png" alt="Windows Sandbox Logo">

Windows Sandbox is a lightweight desktop environment that allows you to run applications in isolation from your host operating system. It's a safe space to test and debug apps, explore unknown files, or experiment with tools without risking your host OS. *Software installed inside the Windows Sandbox environment remains "sandboxed" and runs separately from the host machine.*

Windows Sandbox is a type 2 hypervisor. It uses a unique scheduling policy that allows the virtual processors of the sandbox to be scheduled like threads in a process. This means that the host manages Windows Sandbox as a process, which makes the host more responsive.

Here are some features of Windows Sandbox: 

**Disposable**
*When you close the sandbox, all the software, files, and state are deleted.* 

**Pristine**
*Each time you run the sandbox, it's as clean as a brand-new installation of Windows.* 

**Secure**
*Uses hardware-based virtualization for kernel isolation.* 

**Efficient** 
*Uses an integrated kernel scheduler, smart memory management, and virtual GPU.*

**Battery pass-through**
*Windows Sandbox is aware of the host's battery state and optimizes its power consumption.*

Windows Sandbox is built into Windows 10 Pro and Enterprise, and later versions like Windows 11 Pro and Enterprise. 

---

### Hyper-V

<img width="400px" src="./assets/logosImages//hypervlogo.png" alt="Hyper-V Logo">

Hyper-V is a Microsoft product that allows users to create and run virtual machines (VMs) on a physical host computer. VMs are software versions of computers that can run operating systems and programs, and act like fully functional computers. 

Hyper-V uses a hypervisor, which is software that creates an abstraction layer between the virtual OS and the physical host machine. This allows multiple VMs to run on the same physical machine.

*Hyper-V is considered a Type 1 hypervisor (or bare-metal hypervisor) because it runs directly on the
host's hardware. Hyper-V installs on Windows but runs directly on the physical hardware, inserting itself underneath the host OS. It creates isolated partitions in which operating systems can operate.*

Hyper-V offers several benefits, including:

**Flexibility**
*Users can run more than one operating system on the same hardware, which can help save time and money.* 

**Isolation**
*Each VM runs in its own isolated space, which can help prevent crashes from affecting other workloads.* 

**Performance**
*By eliminating the overhead of a host operating system, Type 1 hypervisors like Hyper-V
typically offer better performance for virtual machines.*

**Direct Hardware Access**
*Hyper-V interacts directly with the physical hardware, allowing for efficient resource
management and performance.*

**Disaster recovery**
*Hyper-V Replica can asynchronously replicate VMs from a primary host to a secondary host, which can help with disaster recovery.* 

**Scalability**
*Hyper-V can manage a large number of virtual machines effectively, making it suitable for
enterprise environments.*

**Hardware utilization**
*Hyper-V can help users make better use of their hardware by consolidating more computing jobs onto less hardware.* 

**Support for Multiple Operating Systems**
*It can host various guest operating systems, including different versions of Windows and Linux.*

Hyper-V is included in many versions of Windows 11. 

Here are some important concepts related to Hyper-V:

**Hypervisor Types**
- **Type 1 (Bare-metal)**: Runs directly on hardware (e.g., Hyper-V).
- **Type 2 (Hosted)**: Runs on an operating system.

**Virtual Machines (VMs)**
- A VM is an emulation of a physical computer, running an operating system and applications.

**Virtual Hard Disks (VHD/VHDX)**
- **VHD**: Virtual hard disk format, limited to 2 TB.
- **VHDX**: Enhanced format, supports up to 64 TB, better performance, and resilience to power
failures.

**Virtual Switches**
- Networking component allowing VMs to communicate with each other and the external
network.
- Types: External, Internal, and Private.

**Resource Management**
- **Dynamic Memory**: Allocates memory dynamically based on demand.
- **CPU Allocation**: Configurable resources for VM performance.

**Checkpoints**
- Snapshots of the VM state, allowing rollback to a previous state for backup or testing.

**Live Migration**
- Moving a running VM from one host to another without downtime.

**High Availability (HA)**
- Ensures VMs are available in case of hardware failure, often using Failover Clustering.

**Replication**
- Hyper-V Replica allows you to replicate VMs to a secondary site for disaster recovery.

**Integration Services**
- Drivers and services that enhance VM performance and provide better interaction with the host
OS.

**Storage Options**
- Different storage types like SMB, iSCSI, and direct attached storage for VMs.

**Windows Server Roles**
- Hyper-V is a server role in Windows Server that enables virtualization.

**PowerShell and Management Tools**
- PowerShell commands and tools like Hyper-V Manager for automation and management.

**Networking Features**
- **NIC Teaming**: Combines multiple network adapters for redundancy and performance.
- **Network Virtualization**: Isolates network traffic between VMs.

**Security Features**
- **Secure Boot**: Protects the VM against boot-time attacks.
- **Shielded VMs**: Provides additional security for sensitive workloads.

---

