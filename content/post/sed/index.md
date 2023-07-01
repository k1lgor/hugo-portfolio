---
title: Mastering the sed Command with Tips, Tricks, and Examples
subtitle: Text Transformation Wizardry

# Summary for listings and search engines
summary: Text Transformation Wizardry

# Link this post with a project
projects: []

# Date published
date: '2023-01-28T00:00:00Z'

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
The `sed` command, short for "stream editor", is a powerful tool in Linux that allows you to perform fundamental text transformations on an input stream, such as a file or input from a pipeline. This blog post will explore some of the most common uses of the `sed` command and provide examples and tips to help you use it more effectively.

### **_Replacing text_**
One of the most common uses of the `sed` command is to replace text in a file. For example, to replace all occurrences of the word "old" with the word "new" in a file called "file.txt", you can use the following command:

![replacing-text-before](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/du24fy6nqq5ze6xrotu8.png)

```
sed 's/old/new/g' file.txt
```

![replacing-text-after](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/4mnxa014d0dyvb5ndg6u.png)

### **_Deleting text_**
Another common use of `sed` is to delete specific lines or text from a file. For example, to delete all lines that contain the word "delete" in a file called "file.txt", you can use the following command:

![deleting-text-before](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/ialte4n9gij88pa6yli9.png)

```
sed '/delete/d' file.txt
```

![deleting-text-after](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/t7f1hc863lbdeuspppma.png)

### **_Inserting text_**
`sed` can also be used to insert text at a specific line number. For example, to insert the text "new line" at line 5 in a file called "file.txt", you can use the following command:

![inserting-text-before](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/xxzcbjmgf2nz99b3my8j.png)

```
sed -n 's/.*\([A-Za-z0-9._%+-]*@[A-Za-z0-9.-]*\.[A-Za-z]*\).*/\1/p' file.txt
```

![inserting-text-after](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/yjx3vlnu5hkmobo238em.png)

### **_Tips and Tricks_**
When working with `sed`, it's important to remember that it can be used to make changes in place, save changes to a new file, or even be used in combination with other commands. For example, you can use the `-i` option to make changes to a file in place, or you can use the `>` operator to save the output of a `sed` command to a new file.

I am gonna use the above example. After executing the last command we can see that the file remains unchanged.

![tips](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/1qfe82ifkygshw5xi04m.png)

Now after executing the same `sed` command but with `-i` option, we will see that the file is changed:

![tips](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/ndcek8dntm63csps1q5b.png)

### **_Conclusion_**
In conclusion, `sed` command is a powerful tool for performing basic text transformations on the input stream, it can be used for replacing, deleting, and inserting text, and even advanced usage with regular expression. By using the above examples and tips, you can use `sed` more effectively to automate your workflow and manage your files.

**_Thank you for reading_** 🧑‍💻

**_Stay tuned for more_** 🚀

✌️ and **_logout_**

<a href="https://www.buymeacoffee.com/k1lgor" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" style="height: 60px !important;width: 217px !important;" ></a>
