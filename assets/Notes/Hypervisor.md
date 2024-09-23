# Hypervisor

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
