---
language: wren
filename: learnwren.wren
contributors:
  - ["Jeremy Ottley", "https://github.com/jeremyottley"]
---

```wren

//// This is a comment.

//// Block comments start with /* and end with */. They can span multiple lines:
/* This 
   is 
   a 
   multi-line 
   comment. */

//// Unlike C, block comments can nest in Wren:
/* This is /* a nested */ comment. */

//// Reserved Words
break class construct else false for foreign if import 
in is null return static super this true var while

//// Identifiers
// Naming rules are similar to other programming languages. Identifiers start with a letter or underscore and may contain letters, digits, and underscores. Case is sensitive.

hi 
camelCase 
PascalCase 
_under_score 
abc123 
ALL_CAPS

// Identifiers that start with underscore (_) are special in Wren. They are used to indicate fields in classes.

//// Newlines
// Newlines (\n) are meaningful in Wren. They are used to separate statements:
// Two statements:
System.print("hi") // Newline.
System.print("bye")

// Sometimes, though, a statement doesn’t fit on a single line and jamming a newline in the middle would trip it up. To handle that, Wren has a very simple rule: It ignores a newline following any token that can’t end a statement.

System.print( // Newline here is ignored.
    "hi")

//// Blocks
// Wren uses curly braces to define blocks. You can use a block anywhere a statement is allowed, like in control flow statements. Method and function bodies are also blocks. For example, here we have a block for the then case, and a single statement for the else:

if (happy && knowIt) { 
  hands.clap() 
} else System.print("sad")

// Blocks have two similar but not identical forms. Typically, blocks contain a series of statements like:
{ 
  System.print("one") 
  System.print("two") 
  System.print("three") 
}

// Blocks of this form when used for method and function bodies automatically return null after the block has completed. If you want to return a different value, you need an explicit return statement.




```
