<h1>A LateX webassembly compiler alongisde an editor</h1>

This is a "LatexEditorBlock" that allows the user to write some LateX text, that can include library and to compile it into an SVG by simply clicking "Validate" button.

The block is re-editable and can be updated very efficiently. LaTeX code is compiled on users's side using XeteX and webassembly.

This is a good component to build a LateX online editor that doesn't require server-side compilations.

This can also be used alongside other of my components to build a multi-support editor.
You can check out my python editor component, geogebra, live musis and others components. 

This component relies on Pdf2svg to transform the compiled pdf into an svg since pdf is not as easy to use as svg in a front-end context.

2 Components are necessary: PdfLatex.razor that uses a webassembly module to compile latex strings to pdf.
This component is an engined that can be called by any LateX block editor component.
It must be loaded before any block.
LatexBlockEditor is a component that is an editable block that can be compiled and edited as much as you want. 

You will find a detailed example of implementation in "Example.Razor" 
