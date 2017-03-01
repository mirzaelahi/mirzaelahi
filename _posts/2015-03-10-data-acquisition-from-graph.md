---
layout: post
title: 'Data Acquisition from Graph'
author: Mirza
tags: [tutorial, matlab]
categories: blogs
excerpt:
  Learn how to extract data from a figure
---

We face many problems in comparing our results with a published paper. To acquire data from a image file of the graph, one may use this method.

-   Download the [digitize2.m](http://www.mathworks.com/matlabcentral/fileexchange/928-digitize2-m) (Authors: A. Prasad, Original version created by J.D.Cogdell).

>There is a bug in this file.

-   In `Line-273` of `digitize2.m` file, replace the below line.

{% highlight matlab%}
if (writefname == 0) || (writepname == 0)
{% endhighlight %}
<!--```Matlab-->
<!--if (writefname == 0) || (writepname == 0)-->
<!--```-->

with
{% highlight matlab%}
if (writefname == 0)
{% endhighlight %}
<!--```Matlab-->
<!--if (writefname == 0)-->
<!--```-->
-   Now, keep your image file and the digitize2.m file in the same folder.
Write a matlab script (.m) to call the function with the image file name as the input.

{% highlight matlab%}
digitize2(‘filename.ext’);
{% endhighlight %}

Here, `ext = jpg, png, tif, bmp, gif`.
Run the script.

-   Follow the instructions showed in the window. At last, Save the data.
-   Load the data in your script if you wish.

{% highlight matlab%}
load(‘FileName.dat’);
{% endhighlight %}

-   You are ready to go.
