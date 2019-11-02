# A quick guide to MARKDOWN language:

|  R   |              Action              |                          Character                           |                        Markdown Code                         |                       Rendered Output                        |
| :--: | :------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: |
|  1   |    **Emphasis** or **Italic**    |               asterisks `*` or underscores `_`               |                     `*text*` or `_text_`                     |                            *text*                            |
|  2   |      ‌‌**Strong** or **Bold**      |                       Two `**` or `__`                       |                   `**text**` or `__text__`                   |                           **text**                           |
|  3   |       **Escape** character       |                        backslash `\`                         |                          `\*text\*`                          |                           \*text\*                           |
|  4   |     **Bold** and **Italic**      |                          Three `*`                           |                         `***text***`                         |                          ***text***                          |
|  5   |          **Line break**          |                        backslash `\`                         |                  `text line1 \ text line 2`                  |                   text line1\ text line 2                    |
|  6   |           **Headings**           |          The more hash `#`, the smaller the header           |                    `### Header number 3`                     |                     ### Header number 3                      |
|  7   |         **Blockquotes**          |              start a line with greater than `>`              |                      This is a `>Quote`                      |                       This is a >Quote                       |
|  8   |      **Nested Blockquotes**      |    Add a `>>` in front of the paragraph you want to nest     |            `>Blockquotes > >>nested Blockquotes`             |             >Blockquotes > >>nested Blockquotes              |
|  9   |       **Unordered lists**        |        either asterisks `*`, plus `+`, or hyphens `-`        |                  List:  `* part 1 * part 2`                  |                   List:  * part 1 * part 2                   |
|  10  |        **Ordered lists**         |      numbers followed by period `.` or right paren `)`       |                    `1. Line 1 2. Line 2`                     |                     1. Line 1 2. Line 2                      |
|  11  |         **Inline link**          |                        `[text](URL)`                         |                `[google:](http://google.com)`                |                 [google:](http://google.com)                 |
|  12  |            **Links**             |                         `text <URL>`                         |                `google: <http://google.com>`                 |                 google: <http://google.com>                  |
|  13  |     **Reference style link**     |            `[text][Ref. No.]<br/>[Ref. No.]:URL`             |        `[hurricane][1]<br/>[1]:https://goo.gl/YEEHP0`        |         [hurricane][1]<br/>[1]:https://goo.gl/YEEHP0         |
|  14  |            **Image**             |                         ![alt](URL)                          |  `![Logo][1]<br/><br/>[1]: https://google.com/favicon.png`   |    [Logo][1]<br/><br/>[1]: https://google.com/favicon.png    |
|  15  |         **Inline code**          |                     Inline code  `code`                      |                                                              |                                                              |
|  16  | **Code block** or **code fence** | 3 backticks on a single line ````` marks the beginning and end of a code block | ```var i;<br/>for (i=0; i<5; i++) {<br/>  console.log(i);}``` | ```var i;<br/>for (i=0; i<5; i++) {<br/>  console.log(i);}``` |
|  17  |            **Indent**            |                  indent 4 spaces or one tab                  | `Who ate the most donuts this week?<br/><br/>    Jeff  15<br/>    Sam   11<br/>    Robin  6` | Who ate the most donuts this week?<br/><br/>    Jeff  15<br/>    Sam   11<br/>    Robin  6 |
|  18  |      **EOL **(End of Line)       |                         `Enter key`                          |                                                              |                                                              |
|  19  |                                  |                                                              |                                                              |                                                              |
