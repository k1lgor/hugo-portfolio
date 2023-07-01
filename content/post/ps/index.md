---
title: Using the ps Command
subtitle: Efficiently Managing Processes with ps

# Summary for listings and search engines
summary: Efficiently Managing Processes with ps

# Link this post with a project
projects: []

# Date published
date: '2023-03-23T00:00:00Z'

# Date updated
lastmod: '2023-03-23T00:00:00Z'

# Is this an unpublished draft?
draft: false

# Show this page in the Featured widget?
featured: false

# Featured image
# Place an image named `featured.jpg/png` in this page's folder and customize its options here.
image:
  # caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/CpkOjOcXdUY)'
  focal_point: ''
  placement: 2
  preview_only: false

authors:
  - admin

tags:
  - Linux
  - Bash
  - Beginners

categories:
  - Blog
---

---

### ***Introduction***

The `ps` command is a powerful tool in Linux that allows you to monitor and manage processes on your system. Whether you need to identify a specific process, check the resource usage of a program, or kill a process that's misbehaving, the `ps` command has you covered.

### ***Using the `ps` Command***

At its simplest, the `ps` command allows you to view information about the processes running on your system. For example, you can use the `ps` command with no options to display a list of all the processes running on your system:

```bash
ps

```

![Image 1](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/r4f39n761o1x565zf4ej.png)

The above command will display a list of all the processes currently running on your system. By default, the `ps` command will display the process ID (PID), the terminal associated with the process, the CPU usage, and the command that started the process

### ***Options and Customization***

While the basic ps command is useful, there are many options and customization features that you can use to tailor the output to your specific needs. For example, you can use the -e option to display information about all processes on the system, regardless of who owns them:

```bash
ps -e
```

![Image 2](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/50b0p9ym2tigz8k2m9om.png)

Another useful option is the -f option, which displays a more detailed output that includes the UID, PPID, C, STIME, TTY, and TIME fields:

```bash
ps -f
```

![Image 3](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/y9w4kdhe8hfklt9afhua.png)

### ***Tips and Tricks***

- You can use the `grep` command to search for specific processes. For example, to search for all processes containing the word "chrome", you can use the following command:

```bash
ps -ef | grep brave

```

![Image 4](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/5z7rp2mirdxwwgm459wp.png)

- You can use the `kill` command to terminate a process. For example, to kill a process with a specific PID, you can use the following command:

```bash
kill PID
```

![Image 5](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/b6eq332ps27voa6jdktk.png)

And you choose the PID number.

- Show all processes with full information:

```bash
ps -ef
```

![Image 6](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/8pdjzn7936bpq70hhgvb.png)


- Show all processes with full information and a tree-like format:

```bash
ps -ejH
```

![Image 7](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/0ofueo7h62by4c00ibls.png)


- Show all processes with full information and a BSD-style format:

```bash
ps axo pid,tt,user,fname,tmout,f,wchan
```

![Image 8](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/044ja1xhx3sagjcjw413.png)


- Show all processes with full information and display the username and start time:

```bash
ps -eo user,pid,ppid,c,start_time,cmd
```

![Image 9](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/k7gsgwe0mkkv1fp9qqop.png)


- Show all processes with full information and display the threads for each process:

```bash
ps -eLf
```

![Image 10](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/mjx3yacnm8fmhbp8nk0x.png)


- Show all processes with full information and display the start time and elapsed time for each process:

```bash
ps -eo pid,comm,lstart,etime
```

![Image 11](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/jtmdzb9smcl3ej5e3n1v.png)


- Show all processes with full information and sort by memory usage (descending):

```bash
ps -e --sort=-rss
```

![Image 12](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/emrysjvy46ckjlwqcauo.png)


- Show all processes with full information and display only the processes owned by a specific user:

```bash
ps -u username
```

![Image 13](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/1dzqed7iavm9xhx2k7qz.png)


- Show all processes with full information and display only the processes with a specific name:

```bash
ps -C program_name
```

![Image 14](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/anpfhmfwxcfq388wiphj.png)


- Show all processes with full information and display only the processes with a specific PID:

```bash
ps -p PID
```

![Image 15](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/qrsu9aoe7zo8bsdwsaft.png)


- You can use the `top` command to view a dynamic real-time display of the processes running on your system.

### ***Conclusion***

The ps command is a powerful and essential tool in Linux for monitoring and managing processes. With its simple syntax and powerful options, you can quickly identify, monitor, and manage processes on your system. Whether you're a system administrator, developer, or power user, the ps command is a must-know tool for efficient Linux management.

***Thank you for reading*** 🧑‍💻

***Stay tuned for more*** 🚀

✌️ and ***logout***

<a href="https://www.buymeacoffee.com/k1lgor" target="_blank">
<img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" >
</a>
