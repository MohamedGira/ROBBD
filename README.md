**[ROBBD Checker]{.ul}**

The purpose of this project is to create a ROBDD constructor. It has
various features such as visualization and comparisons between different
techniques such as Truth table or ROBDD comparison.

**[Pre-requisites]{.ul}**

In order to be able to use this program you first need to do the
following:

1.  Install Graphviz library ( pip install graphviz)

2.  Visit <https://graphviz.org/download/> and download the version
    suitable for your machine

    -   Note: on installation, you must tick "add to PATH" check box in
        order for it to work.

**[Usage]{.ul}**

You can create ROBDD objects and construct them using " construct()
"method by passing any Boolean expression in similar formats as follows


* `" A'B' + A'B + AB' + AB " `
* `" abc + b'c + ca +b' " `
* `" A * B  + ! A * C + A * ! B * C  "`
* `" A'C' + C'D + AC + CD'  "`
* `" A'C' + AD + CD'  "`
* `" A * B * C + ! A + A * ! B * C"`
* `" ( NOT D XOR C ) AND ( B XOR A ) AND ( E OR ! E ) * ( E OR F ) AND G XOR XND * Y OR Z OR V OR N OR C " # will take long time`
*  `" ( a * b + ! a * ! b ) AND ( c * d + ! c * ! d ) "`
*  `" ! ( ! ( ! A ) ) "`
*  `" ( C ^ D ) AND ( B XOR A ) "`


You can visualize the graph as follows using `visualize_graph()` which takes string expression as an input.


**[output]{.ul}**

![](media/image3.png)
you can use g.render(filename,
file_path,auto_view) to customize file output

![](media/image4.png)
you can also use compare_expressions(exp1,exp2) to
visualize and compare 2 different expressions

![](media/image5.png)
![](media/image6.png)

![Text Description automatically
generated](media/image7.png)
![](media/image8.png)
![](media/image9.png)
