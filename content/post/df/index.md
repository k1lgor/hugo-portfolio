---
title: Managing Disk Space in Linux with the df Command
subtitle: Unlocking Disk Space Secrets

# Summary for listings and search engines
summary: Unlocking Disk Space Secrets

# Link this post with a project
projects: []

# Date published
date: '2023-03-09T00:00:00Z'

# Date updated
lastmod: '2023-03-09T00:00:00Z'

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

### **_Introduction_**

The `df` command is a Unlocking Disk Space Secrets. It displays information about the file system disk space usage, including the amount of free space, used space, and the percentage of space used. Here are some examples of using `df` command:

### **_Show disk space usage in human-readable format_**

```bash
df -h
```

![Image 1](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/s5ap8or48ghh4g4m6l8f.png)

### **_Show disk space usage for a specific file system_**

```bash
df -hT /dev/sda1
```

![Image 2](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/2smwkc15uqydtn37411w.png)


### **_Show disk space usage for all file systems (including speudo file systems)_**

```bash
df -aTh
```

![Image 3](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/ql0e18882kgm3pjsoo3s.png)


### **_Show disk space usage for a specific file system and exclude file systems of a certain type_**

```bash
df -hT -x tmpfs /dev/sda1
```

![Image 4](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/5p9wn42nqnrzs9oj44yx.png)


### **_Show disk space usage in bytes for all file systems (including empty file systems)_**

```bash
df -BT
```

![Image 5](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/aclcnelaf3rkp6hc5wkf.png)


### **_Show disk space usage for a specific file system with inode information_**

```bash
df -i /dev/sda1
```

![Image 6](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/9zjqyg5y9g02joxl9lad.png)


### **_Show disk space usage with a specific output format_**

```bash
df --output=source,fstype,size,used,avail,pcent,target
```

![Image 7](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/i9yq3380ay5y19vi3tjm.png)


### **_Show disk space usage sorted by a specific column (ascending)_**

```bash
df -hT | sort -k 3
```

![Image 8](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/p5be4y1br1ptfgmlk3sp.png)


### **_Show disk space usage sorted by a specific column (descending)_**

```bash
df -hT | sort -k 3 -r
```

![Image 9](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/xkdfjpr128bgncr421q7.png)


### **_Show disk space usage for all file systems and exclude the header line_**

```bash
df -hT | tail -n +2
```

![Image 10](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/mrqecndg8i0wbv32nc9w.png)


### **_Tips_**

- Use the `h` option to display disk space usage in human-readable format (e.g., GB, MB)
- Use the `x` option to exclude file systems of a certain type (e.g., tmpfs,devtmpfs)
- Use the `-output` option to customize the output format of the command
- Use the `sort` and `tail` commands to sort and filter the output as needed.

### **_Conclusion_**

In summary, the `df` command is a powerful tool for managing disk space on your Linux system. With the various options available, you can easily view and analyze disk space usage for specific file systems and customize the output format.
Remember to use the available sorting and filtering commands to further manage and analyze the output.

**_Thank you for reading_** 🧑‍💻

**_Stay tuned for more_** 🚀

✌️ and **_logout_**

<a href="https://www.buymeacoffee.com/k1lgor" target="_blank">
<img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" >
</a>
