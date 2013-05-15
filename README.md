# IE-Media-Queries #
A simple script to use media queries in IE 8 and lower.
## Usage ##
Simply insert the following Javascript into the <head> of your document.

    <!--[if lt IE 9]>
    <script type="text/javascript">
    var headID = document.getElementsByTagName("head")[0]; 
    var cssNode = document.createElement('link');
    if (document.documentElement.clientWidth > "min screen size here" {
    cssNode.type = 'text/css';
    cssNode.rel = 'stylesheet';
    cssNode.href = 'Your css file here';
    cssNode.media = 'screen';
    headID.appendChild(cssNode);
    }
    </script>
    <![endif]-->

You can change the > to a < to indicated a maximum screen size for a specific stylesheet.