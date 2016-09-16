# bpmn-js-utils

Collection of Javascript and HTML using bpmn.js

#### /src/tab_js_browserified.js

Javascript library for rendering BPMN 2.0 XML into svg. Reads the XML from the property "bpmn20Xml" of the given object. Injects the generated SVG into a div with the id "js-canvas".

Including and calling:

      var bpmnUtil = window.tabjs;

      bpmnUtil.showBpmnCallback(object);

#### /src/bpmn-js.html

Needs to be configured in the file.

Test page where you can paste XML to have it rendered.

#### /src/bpmn-iframe.html

Needs to be configured in the file.

Page that loads the XML file from a given URL and renders it.

i.e. "http://host:port/bpmn-iframe.html?url=http://..."

Also supports highlighting of tasks in the workflow, referenced by their definition "key".

i.e. "http://host:port/bpmn-iframe.html?task=UserTask_1&url=http://..."

Configuration:

In both HTML files there is a external Javascript reference which has to be set to the script's location.