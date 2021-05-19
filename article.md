
# Section (H1) 

Paragraph text, typical writing in regular ye olde people's English.

## Sub-Section (H2)

Include a figure with a caption: 

![homer](fig/homer.png "Homer's Reaction")

Refer to that figure:

Figure~\ref{fig:homer} shows (blah blah blah).  

## Another Sub-Section

* Bullet
* List
* Without insane Latex nerdery

A horizontal bar (not that we make those):  

---

Code:

```verilog
module WHY #( /* ... */ ); 
  generate
  for (k=0; k<WIDTH; k=k+1) begin
    fa i_fa( /* ... */ );
  end
  endgenerate 
endmodule
```

Citation: [@latexcompanion] 

Inline code: `print("...")`  

Link: [overleaf.com](https://www.overleaf.com)  

Tables, sadly, must be specified in Latex and not Markdown. An example below from the template's `main.tex` front-page file. 

