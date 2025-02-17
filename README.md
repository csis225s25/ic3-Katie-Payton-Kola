# In Class Problem Set 3

I used ComboBoxDemo.java a few years ago.  It used to compile cleanly.  Even though the code has not changed, it now  will not compile without throwing warnings.

Doing everything from a command prompt or Git Bash (no IDEs allowed), your mission is to debug the code and find out why it stopped compiling cleanly.  When you have figured it out,  note what you changed and why it stopped working in the README.md file.

Katie, Payton, Jaden, and Kola

**Changes to code**
Change from 
    static JComboBox cBox1;
    cBox1 = new JComboBox(s1);

  to:
   static JComboBox<String> cBox1;
   cBox1 = new JComboBox<String>(s1);


**What caused it to stop working?**
Uses unchecked or unsaved operations
The compiler can't check if we are using the JComboBox with the right type, so we need to state the type of object we are storing in the collection.
