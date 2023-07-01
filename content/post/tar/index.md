---
title: Compressing and Archiving Files with tar
subtitle: Examples and Tips

# Summary for listings and search engines
summary: Examples and Tips

# Link this post with a project
projects: []

# Date published
date: '2023-02-11T00:00:00Z'

# Date updated
lastmod: '2023-02-22T00:00:00Z'

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
The `tar` command is one of the most commonly used tools in Linux for compressing and archiving files. With `tar`, you can combine multiple files into a single archive file, and also extract files from an archive. In this blog post, we'll explore the basics of the `tar` command, as well as some advanced techniques and examples to help you get the most out of this powerful tool.

### **_Basic Usage_**
The most basic use of `tar` is to create an archive file from one or more files. For example, to create an archive named "example.tar" from two files named "file1.txt" and "file2.txt", you would use the command:

```
tar -cvf example.tar file1.txt file2.txt
```

![Image 1](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/frla36d6i9hjj5a0duff.png)

![Image 2](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/70zjx2vagf7qcznjp5ha.png)

The options used in this command are: `c` for create, `v` for verbose (displays the names of files being added to the archive), and `f` for file, which specifies the name of the archive to be created.

### **_Compression Options_**
By default, `tar` does not compress the archive file. However, you can specify a compression format to be used with the `z` or `-gzip` option for gzip compression, or the `j` or `-bzip2` option for bzip2 compression.

For example, to create a gzip-compressed archive named "example.tar.gz" from two files named "file1.txt" and "file2.txt", you would use the command:

```
tar -zcvf example.tar.gz file1.txt file2.txt
```

![Image 3](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/gwpj8uig58bbt53wmedf.png)

### **_Extracting Files from an Archive_**
To extract the files from an archive, you can use the `x` option. For example, to extract the contents of the archive "example.tar", you would use the command:

```
tar -xvf example.tar
```

![Image 4](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/fwwdphjbq2ublokqo4lh.png)

The `v` option can be used to display the names of the files being extracted from the archive.

### **_Listing the Contents of an Archive_**
To display the contents of an archive without extracting the files, you can use the `t` option. For example, to list the contents of the archive "example.tar", you would use the command:

```
tar -tvf example.tar
```

![Image 5](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/jhpsneoleho8gxr9vxf5.png)

### **_Updating an Archive_**
To add new files to an existing archive, or update existing files in the archive, you can use the `u` or `-update` option. For example, to add a file named "file3.txt" to the archive "example.tar", you would use the command:

```
tar -uvf example.tar file3.txt
```

![Image 6](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/pkjcz5ssmxkrqad78qls.png)

### **_Conclusion_**
These are just a few examples of how to use the `tar` command. With its options for compression and archive updates, `tar` is a powerful tool for compressing and archiving files in Linux.

**_Thank you for reading_** 🧑‍💻

**_Stay tuned for more_** 🚀

✌️ and **_logout_**

<a href="https://www.buymeacoffee.com/k1lgor" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>
