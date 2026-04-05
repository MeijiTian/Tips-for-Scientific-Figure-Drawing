## Tips for Scientific Figure Drawing

 I would like to share some practical experience I have gained from preparing figures for ML/CV conference and journal papers.

 # Overview
In my view, a well-designed scientific figure usually depends on the following three aspects:

1. **Format**: All figures should maintain a consistent visual style, including font size, color scheme, and layout. Before pursuing aesthetics, readability should always come first.
2. **Font**: **Sans-serif** fonts are generally recommended, such as `Arial`, `Aptos`, or `Myriad Pro`. The font size in figures should satisfy submission requirements and is usually not smaller than the body text by more than one size level.
3. **Color**: It is generally better to limit the main colors in a figure to no more than three, and choose colors according to the meaning you want to convey.
   + If you want to highlight contrast, use contrasting colors.
   + If you want to show hierarchy or continuity, use colors from the same palette with gradual variation.


  
## 1. Prepare Your Canvas
+ Many researchers use PowerPoint to create scientific figures. The first step is to set the **canvas size** based on the template of your target venue. For either single-column or double-column figures, it is helpful to set the canvas width equal to the template width, or to an integer multiple of it. This makes it easier to control font size and helps ensure that the text in the figure remains visually consistent with the main paper after insertion.
+ After finishing the figure, export it as a **high DPI PDF** and insert it into your LaTeX manuscript.

## 2. Method Diagrams and Teasers
+ Avoid placing too much text inside the figure. Try to replace long descriptions with symbols or concise visual cues, and move detailed explanations to the caption. That said, **readability should always come first**, and simplicity should never introduce ambiguity.
+ Mathematical symbols: equations created directly in PowerPoint are often not visually pleasing. I recommend using an online LaTeX equation editor, rendering the equation as an SVG, and then importing it into the figure. A useful website is [LaTeX Live Equation Editor](https://www.latexlive.com/).
+ Borders and arrows: a flat visual style is generally a good choice and aligns well with current design preferences. Rounded rectangles and rounded-tail arrows usually look cleaner. You can also add subtle shadows when appropriate to create a mild sense of depth.
+ Fonts: keep the text easy to read, and if possible, use only one font family throughout the figure. Differences can be introduced through bold or italic styles rather than switching fonts.

## 3. Comparative Result Figures
+ Keep each result panel at a reasonable and consistent size. For example, in a single-column figure, it is usually better not to place more than **seven images** in one row.
+ When showing error maps, use a consistent colormap from the same palette. I generally do not recommend using `jet`, because its abrupt color transitions can interfere with intuitive visual comparison.
+ Add a **color bar** when needed so that the meaning of the values is clear to the reader.
+ Method names should be clearly readable. It is often helpful to explicitly label your own method as `(Ours)`.
+ Preserve the original aspect ratio of the images. For medical images in particular, follow **standard radiological display conventions** when arranging them. 
   - For example, avoid flipping the brain upside down or reversing the orientation of the chest and back.

## 4. Line Charts and Statistical Plots
+ Line charts: use clearly distinguishable colors and markers to differentiate different curves.
+ Box plots: different textures or fill patterns can help separate groups more effectively.
+ Color choice: use colors from the same palette for progressive relationships, and use contrasting colors when you want to emphasize differences.

## 5. Choosing Colors
+ Keep the overall visual style consistent. 
  - For example, the colors used in result figures should match the visual language used in method diagrams.
+ Choose colors based on the meaning you want to convey. Color semantics matter: for instance, red often suggests warning or emphasis, while green is commonly associated with safety or normality.


## Acknowledgement

+ [JCI Figure Guidelines](https://www.jci.org/kiosks/publish/figures)
+ Bilibili: `学术论文作图规范`
   - [Mandatory Requirement](https://www.bilibili.com/video/BV1QoCAYCEwa/)
   - [Color Scheme (I)](https://www.bilibili.com/video/BV1fbwveoEWo/)
   - [Color Scheme (II)](https://www.bilibili.com/video/BV1C54nzmEdX/)
