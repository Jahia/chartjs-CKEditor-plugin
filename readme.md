# chart.js CKEditor plugin

This plugin is adding the possibility to create chart form CKEditor in Digital Factory, it's based on [chart.js](https://www.chartjs.com) library.

### INSTALLATION

To install this plugin you need to copy the chart folder to your ckeditor module under `javascript/plugins`,
 then deploy your CKEditor module and go to `Jahia tools > CKEditor Custom Configuration`
 and add `'widget,lineutils,chart'` to `config.extraPlugins` and `,'ChartBar','ChartRound'` to `config.toolbar_Full[8]`.
 Or simply copy the following example :

```
    CKEDITOR.editorConfig = function( config ) {
        config.extraPlugins='widget,lineutils,chart';
        config.toolbar_Full[8]=['Image','Flash','Table','HorizontalRule','Smiley','SpecialChar','PageBreak','ChartBar','ChartRound'];
    }
```

**Carefull**
This is an example if you already have your own CKEditor configuration, you will have to adapt it!