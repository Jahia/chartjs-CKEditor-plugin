# chart.js CKEditor plugin

This plugin is adding the possibility to create chart from CKEditor in Digital Factory, it's based on [chart.js](http://www.chartjs.org) library.

### INSTALLATION

To install this plugin you need to copy the chart folder to your ckeditor module under `javascript/plugins`,
 then deploy your CKEditor module and go to `Jahia tools > CKEditor Custom Configuration`
 and add `'widget,lineutils,chart'` to `config.extraPlugins` and `,'ChartBar','ChartPie'` to `config.toolbar_Full[8]`.

You will also need to add the following line:
`config.protectedSource.push(/<jahia:resource[\s\S\t\r\n]*?\/jahia:resource>/);`

Or simply copy the following example :

```
CKEDITOR.editorConfig = function( config ) {
    config.extraPlugins='widget,lineutils,chart';
    config.toolbar_Full[8]=['Image','Flash','Table','HorizontalRule','Smiley','SpecialChar','PageBreak','ChartBar','ChartPie'];
    config.protectedSource.push(/<jahia:resource[\s\S\t\r\n]*?\/jahia:resource>/);
}
```

**Carefull**
This is an example if you already have your own CKEditor configuration, you will have to adapt it!