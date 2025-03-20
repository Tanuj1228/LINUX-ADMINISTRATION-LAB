# **Experiment - 3 & 4**

_View the gedit man page. Use the `man -k ext4` command to find the command to tune ext4 file-system parameters. Brace expansion is used to generate discretionary strings of characters. Braces contain a comma-separated list of strings, or a sequence expression. The result includes the text that precedes or follows the brace definition._

#

### **Approach**

Use the `man` command to view manual pages and search for commands related to `ext4`. Utilize brace expansion to generate sequences efficiently.

### **Syntax**

**`man [command]`**  
 Displays the manual page for the specified command.

**`man -k [keyword]`**  
 Searches for the keyword in the manual pages and lists all matching entries.

**`echo [pattern]`**  
 Outputs the result of a pattern or variable expansion.

**`echo {start..end}`**  
 Expands a range of values from `start` to `end` and outputs the result.

### **Example**

```
man gedit

```

```
man -k ext4

```

```
echo file{1,2,3}.txt

```

```
echo {a..e}

```

#
![lab2 1](https://github.com/user-attachments/assets/3f2e1a57-d03e-43f9-888d-e0fb62542fae)
#
![lab2 2](https://github.com/user-attachments/assets/b31a0778-6354-4f32-95b1-c366920bbdc1)
#
![lab2 3](https://github.com/user-attachments/assets/5b0db7e3-458a-48cd-8d33-d226c8637771)
