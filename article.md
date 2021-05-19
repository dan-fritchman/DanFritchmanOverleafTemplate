
# Section (H1) 

Paragraph text

## Sub-Section (H2)

Include a figure with a caption: 

![homer](fig/homer.png "Homer's Reaction")

Refer to that figure:
Figure~\ref{fig:homer} shows (blah blah blah)

* Bullet
* List
* Without insane Latex nerdery

Citation: [@genc2019gemmini] 

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

Link: [https://github.com/dan-fritchman/NonAnalogComputeInMemory](https://github.com/dan-fritchman/NonAnalogComputeInMemory)

Tables, sadly, must be specified in Latex and not Markdown. 

