# **Experiment - 5 & 6**

_Use Vim or nano to edit the file named `editing_final_lab.txt`. Utilize the `lab_file` shell variable for referencing the file. In Vim, enter visual mode to manipulate the text efficiently. The objective is to remove the last seven characters from the first column on the first line while ensuring that only the first four characters of the first column remain._

#

### **Approach**

Use `vim` or `nano` to open the file and modify its content. In Vim, visual mode helps in precise text selection and deletion.

### **Syntax**

**`var="file1.ext"`**  
Assigns the file name `"file1.ext"` to the variable `var` for later use in commands.

**`vim $var`**  
Opens the file using Vim with the shell variable.

**`nano $var`**  
Opens the file using Nano with the shell variable.

### **Example**

```
touch editing_final_lab.txt

```

```
lab_file="editing_final_lab.txt"

```

```
nano $lab_file

```

In the nano editor, add the following text:

```
This file is editing_final_lab.txt
This file is stored in Lab-3 directory
Hello World
```

Save and exit nano.

```
vim $lab_file

```

Preserve only the first four characters of the first column:

```
edit
This file is stored in Lab-3 directory
Hello World
```

```
cat editing_final_lab.txt

```

#
