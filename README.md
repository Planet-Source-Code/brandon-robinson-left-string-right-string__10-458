<div align="center">

## Left\(String,?\) Right\(String,?\)


</div>

### Description

Alrighty, Just like everyone else. I am just a little frustrated trying to find all my old fuctionality from VB6 in VB.NET. So when I ran across this I thought I would post it.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Brandon Robinson](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/brandon-robinson.md)
**Level**          |Beginner
**User Rating**    |5.0 (15 globes from 3 users)
**Compatibility**  |VB\.NET
**Category**       |[Coding Standards](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/coding-standards__10-33.md)
**World**          |[\.Net \(C\#, VB\.net\)](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/net-c-vb-net.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/brandon-robinson-left-string-right-string__10-458/archive/master.zip)





### Source Code

<html>
<body>
<TABLE CELLSPACING=0>
<TR ID="hdr">
<TD CLASS="runninghead" nowrap>Visual Basic Language Reference</TD>
<TD CLASS="product" nowrap> </TD>
</TR>
</TABLE>
</div>
<div id="TitleRow">
<H1 class="dtH1"><A NAME="vastmimports"></A>Imports Statement</H1>
</div></div>
<DIV id="nstext" valign="bottom"><!---->
<P>Imports namespace names from referenced projects and assemblies. Also imports namespace names defined within the same project as the file in which the statement appears.</P>
<PRE class="syntax"><B>Imports</B> [ <I>aliasname = </I>] <I>namespace </I>[ <I>. element </I>]</PRE>
<H4 class="dtH4">Parts</H4>
<DL>
<DT><I>aliasname</I></DT>
<DD>Optional. The name by which <I>namespace</I> may also be known or referred to. When the <B>Imports</B> statement does not include <I>aliasname</I>, the elements defined within the specified <I>namespace</I> can be accessed within the file without qualification. When <I>aliasname</I> is specified, it must be used as a qualifier for the names contained in the namespace. Aliases are useful when you need to use items with the same name that are declared in one or more namespaces. </dd>
<DT><I>namespace</I></DT>
<DD>Required. The name of the namespace being imported. The namespace can be any number of nesting levels deep.</dd>
<DT><I>element</I></DT>
<DD>Optional. The name of an element declared in the namespace. The element can be an enumeration, structure, class, or module.</dd>
</DL>
<H4 class="dtH4">Remarks</H4>
<P>Each file can contain any number of <B>Imports</B> statements. <B>Imports</B> statements must be placed before any declarations, including <B>Module</B> or <B>Class</B> statements, and before any references to identifiers.</P>
<P>The scope of the elements made available by an <B>Imports</B> statement depends on how specific you are when using the <B>Imports</B> statement. For example, if only a namespace is specified, all uniquely named members of that namespace, and members of modules within that namespace, are available without qualification. If both a namespace and the name of an element of that namespace are specified, only the members of that element are available without qualification.</P>
<P>It is not permitted to define a member at module level with the same name as an import alias.</P>
<H4 class="dtH4">Example</H4>
<P>The following example imports the <B>Microsoft.VisualBasic.Strings</B> class and assigns an alias, <code class="ce">Str</code>, that can be used to access the <B>Left</B> method.</P>
<PRE class="code"><code><b class="cfe">Imports</b></code> Str = Microsoft.VisualBasic.Strings
' Place Imports statements at the top of your program
Class MyClass1
 Sub ShowHello()
  MsgBox(Str.Left("Hello World", 5)) ' Displays the word "Hello"
 End Sub
End Class</PRE>
</BODY>
</HTML>

