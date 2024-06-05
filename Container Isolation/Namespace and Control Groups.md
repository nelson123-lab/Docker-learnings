Containers achieve isolation primarily through two features in the Linux kernel: **namespaces** and **cgroups (control groups)**.

1. **Namespaces**: Namespaces provide the fundamental basis for container isolation by partitioning kernel resources so that one set of processes sees one set of resources while another set of processes sees a different set of resources. The key types of namespaces include:
   - **PID namespace**: Isolates the process ID number space, so processes in different namespaces can have the same PID.
   - **NET namespace**: Isolates network interfaces, IP addresses, ports, routing tables, and related resources.
   - **MNT namespace**: Isolates filesystem mount points.
   - **IPC namespace**: Isolates inter-process communication resources (e.g., message queues, semaphores).
   - **UTS namespace**: Isolates hostname and domain name.
   - **USER namespace**: Isolates user and group ID ranges.

2. **Cgroups (Control Groups)**: Cgroups provide resource limiting and accounting. They allow the allocation of resources such as CPU time, memory, disk I/O, and network bandwidth among user-defined groups of tasks (processes) running on a system. Key features include:
   - **Resource Limiting**: Control how much of a specific resource (e.g., CPU, memory) can be used by processes within a cgroup.
   - **Prioritization**: Set the priority of resource access for different cgroups.
   - **Accounting**: Track how much of a resource is used by processes within a cgroup.
   - **Control**: Freeze or stop processes within a cgroup.
