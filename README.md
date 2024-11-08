# Cloud Computing

<img src="./assets/logosImages/cloudComputingImage.jpg" alt="Cloud Computing Image">

### Virtualization

Virtualization is a technology that allows a single physical computer or server to be divided into multiple virtual machines, or "VMs". These VMs can then run different operating systems or applications while sharing the resources of the host machine.\
🔗 [Virtualization Notes](./assets/Notes/Virtualization.md)

### Hypervisor

A hypervisor is a software, firmware, or hardware component that allows a single physical machine to run multiple virtual machines (VMs).\
🔗 [Hypervisor Notes](./assets/Notes/Hypervisor.md)

### VMware Workstation

VMware Workstation is a desktop virtualization product that allows users to run multiple operating systems on the same computer without rebooting.\
🔗 [VMware Workstation Notes](./assets/Notes/VMware%20Workstation.md)

### VirtualBox

Oracle VirtualBox is a hosted hypervisor for x86 virtualization.\
🔗 [VirtualBox Notes](./assets/Notes/VirtualBox.md)

### Windows Sandbox

Windows Sandbox is a lightweight desktop environment that allows you to run applications in isolation from your host operating system.\
🔗 [Windows Sandbox Notes](./assets/Notes/Windows%20Sandbox.md)

### Hyper-V

Hyper-V is a Microsoft product that allows users to create and run virtual machines (VMs) on a physical host computer.\
🔗 [Hyper-V Notes](./assets/Notes/Hyper-V.md)

#### 📜 [Tasks Week 2](./assets/Lab/TaskWeek2.md)
- [Basic VM Creation and OS Installation](./assets/Lab/TaskWeek2.md#basic-vm-creation-and-os-installation)
- [Observing Power States of VMs in Hyper-V](./assets/Lab/TaskWeek2.md#observing-power-states-of-vms-in-hyper-v)
- [Networking and Virtual Switches](./assets/Lab/TaskWeek2.md#networking-and-virtual-switches)
- [Snapshot Management](./assets/Lab/TaskWeek2.md#snapshot-management)
- [Resource Allocation and Performance Monitoring](./assets/Lab/TaskWeek2.md#resource-allocation-and-performance-monitoring)

### Scalability

Scalability in Cloud Computing refers to the ability of a cloud system to handle increasing or decreasing workloads efficiently. It allows resources such as processing power, storage, and network bandwidth to expand or contract dynamically based on demand.\
This flexibility ensures that businesses can scale up during peak usage periods and scale down during low-demand times, optimizing costs and maintaining performance. Cloud providers offer two types of scalability:

**Vertical Scalability (Scaling Up)**: Increases the capacity of existing hardware by adding more power (e.g., upgrading to a more powerful server).

**Horizontal Scalability (Scaling Out)**: Involves adding more servers or nodes to distribute the load, which is often preferred for handling high-demand workloads.

*Scalability is a core advantage of cloud computing, enabling businesses to grow without the need for massive upfront infrastructure investments.*

🔗🌐 [Horizontal Vs. Vertical Scaling: Which Should You Choose?](https://www.cloudzero.com/blog/horizontal-vs-vertical-scaling/)

### Security Threats in Virtual Machines

**Security Threats in Virtual Machines (VMs)** arise due to the shared nature of virtualized environments, where multiple VMs run on the same physical hardware. Key threats include:

1. **Hypervisor Attacks**: The hypervisor, which manages VMs, can be a target for attackers. Compromising the hypervisor (e.g., through vulnerabilities) allows attackers to control or access all VMs on the host.

2. **VM Escape**: In this scenario, an attacker exploits a vulnerability in a VM to break out and gain control over the host system or other VMs.

3. **Inter-VM Attacks**: If VMs share resources, an attacker in one VM could exploit side-channel attacks or vulnerabilities to access data from another VM.

4. **Snapshot and Data Leakage**: VM snapshots store the complete state of a VM. If snapshots are not properly secured, sensitive data can be exposed.

5. **Insecure Configuration**: Misconfigured VMs, such as weak access controls or unpatched software, can lead to unauthorized access or exploitation.

Ensuring strong isolation between VMs, securing the hypervisor, and regularly updating and monitoring the virtual environment are key steps in mitigating these threats.

🔗🌐 [What Is System Hardening?](https://blog.netwrix.com/2023/02/22/system-hardening/#:~:text=This%20process%20includes%20removing%20unnecessary,for%20unauthorized%20access%20to%20occur)

### CDN 

CDN stands for content delivery network or content distribution network. It's a system of servers that are spread out around the world to deliver content to users quickly and efficiently.

🔗 [CDN Notes](./assets/Notes/CDN.md)

🔗🌐 [What is a CDN? Content Delivery Network Explained - AWS](https://aws.amazon.com/what-is/cdn/#:~:text=A%20content%20delivery%20network%20(CDN,reaches%20their%20computers%20much%20faster.))\
🔗🌐 [What is a CDN? How does a CDN Work? - Imperva](https://www.imperva.com/learn/performance/what-is-cdn-how-it-works/#:~:text=Website%20Security,of%20your%20core%20network%20infrastructure.)

### Cloud Storage Types

The main types of cloud storage are object, file, and block storage:

**Object storage**\
Pairs data with unique identifiers called metadata. Objects are uncompressed and unencrypted, so they can be accessed quickly at scale.

**File storage**\
Organizes data and represents it to users. It has a hierarchical structure that makes it easy to navigate data, but it also increases processing time.

**Block storage**\
Splits a storage volume into individual instances called blocks. It's a fast storage system with low latency, making it ideal for high performance workloads.

🔗 [Cloud Storage Types](./assets/Notes/CloudStorageTypes.md)

🔗🌐 [What is Cloud Storage? - Cloud Storage Explained - AWS](https://aws.amazon.com/what-is/cloud-storage/#:~:text=There%20are%20three%20main%20cloud,file%20storage%2C%20and%20block%20storage.)


### Auto Scaling in AWS

Amazon Web Services (AWS) Auto Scaling is a free service that automatically scales AWS resources to optimize costs and utilization. It can scale resources for multiple services, including:
- Amazon EC2 instances and Spot Fleets
- Amazon ECS tasks
- Amazon DynamoDB tables
- Amazon Aurora Replicas
- Amazon EMR instances
- Amazon AppStream 2.0 fleets 

AWS Auto Scaling can:
- **Increase resources when demand rises**\
Automatically increase computing power or storage resources when demand increases 
- **Reduce resources when demand drops**
Automatically remove excess resource capacity when demand drops
- **Optimize performance and costs**\
Provide recommendations to optimize performance and costs, or balance between them 
- **Scale based on conditions**\
Scale resources based on conditions you define, such as target tracking, step scaling, or scheduled scaling 
- **Create custom scaling strategies**\
Define how to optimize resource usage, such as preferring availability, cost, or a balance of the two 

*You can use the AWS Management Console, Command Line Interface (CLI), or SDK to get started with AWS Auto Scaling.*

🔗🌐 [AWS Auto Scaling](https://aws.amazon.com/autoscaling/#:~:text=AWS%20Auto%20Scaling%20monitors%20your,across%20multiple%20services%20in%20minutes.)