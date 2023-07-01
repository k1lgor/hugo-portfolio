---
title: Unlock the power of the find command
subtitle: A Beginner's Guide with Examples

# Summary for listings and search engines
summary: A Beginner's Guide with Examples

# Link this post with a project
projects: []

# Date published
date: '2023-01-31T00:00:00Z'

# Date updated
lastmod: '2023-02-12T00:00:00Z'

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

The `find` command is a powerful tool in Linux that allows you to search for files and directories in a specified location. With `find` you can search for files based on their name, type, size, and many other criteria. In this blog post, we will explore some examples of how to use the `find` command, as well as some tips and tricks for getting the most out of it.

### **_Searching for files by name_**

The most basic use of `find` is to search for files by name. For example, to search for all files in the current directory with the name "example.txt", you would use the command:

```
find . -name "example.txt"
```

![image-1](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/iw94isw6s05uut1jj4m1.png)

### **_Searching for files by type_**

You can also search for files by type using the `find` command. For example, to search for all directories in the current directory, you would use the command:

```
find . -type d
```

![image-2](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/ovd9f9lws8pd7pdigxg3.png)

### **_Searching for files by size_**
Another useful option for `find` is the ability to search for files by size. For example, to search for all files larger than 100MB in the current directory, you would use:

```
find . -size +100M
```

![image-3](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/jopz6ufsqg0xzippfj0k.png)

### **_Using logical operators_**

You can use logical operators like `-and`, `-or`, and `-not` to combine different search criteria. For example, to search for all files with the name "example.zip" that are larger than 100MB, you would use the command:

```
find . -name "example.zip" -and -size +100M
```

![image-4](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/7fb59yt6lpydxv6jsogi.png)

### **_Executing commands on found files_**

One of the most powerful features of `find` is the ability to execute commands on the files that it finds. For example, to delete all files in the current directory with the name "example.txt", you would use the command:

```
find . -name "example.txt" -delete
```

![image-5](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/7qptny3anj50im7x43sm.png)

Another example:

```
find . -name "example.txt" -exec rm {} \;
```

![image-6](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/nfsoe8b5zqlso7nn2a6k.png)

The command `find . -name "example.txt" -exec rm {} \;` is used to search for files named "example.txt" starting from the current directory (`.`) and execute the `rm` command on each file found.

- The `find` command is used to search for files or directories that match certain criteria.

- The `.` specifies the directory to start the search from, in this case, it's the current directory.

- The `-name "example.txt"` option specifies the name pattern to search for, in this case, it's "example.txt".

- The `-exec rm {} \;` option specifies the action to be taken on each file found. The `rm` command will be executed on each file found and the file will be passed as an argument to `rm` using `{}`. The `\;` is used to terminate the command.

So, this command will search the current directory and all its subdirectories for files named "example.txt" and remove each file that it finds.

### **_Tips and Tricks_**

`find` command is also capable of searching in a specific directory by specifying the path of the directory to search.

```
find ~/Public -name "example.txt"
```

![image-7](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/ld8bo2srs81erp1bvb3d.png)

### **_Conclusion_**

The `find` command is a powerful tool for searching for files and directories in Linux. With `find`, you can search for files based on their name, type, size, and many other criteria, and even execute commands on the files that it finds.

```
find . -name "*.txt" -exec cat {} \;
```

![image-8](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/nhbgth9px2mdq74ijn1d.png)

**_Thank you for reading_** 🧑‍💻

**_Stay tuned for more_** 🚀

✌️ and **_logout_**

<a href="https://www.buymeacoffee.com/k1lgor" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>
