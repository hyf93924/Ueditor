# Ueditor
Ueditor配置文件   
---   
#### 这是百度编辑器Ueditor的引入（将Ueditor的相关文件复制到ueditor中，即除了ueditor2所有文件复制进去）   
   
##### Ueditor的引入开发可完全参照其官方的开发文档进行开发，在引入文件中：   
- 首先引入编辑器文件     
`<script type="text/javascript" src="../ueditor/editor_config.js"></script>`   
`<script type="text/javascript" src="../ueditor/editor_all.js"></script>`    
- 然后进行编辑器渲染    
`<script type="text/javascript">`    
`myed = new UE.ui.Editor();`    
`myed.render();`    
`</script>`   
- 最后就是在原配置文件中修改项目的路径    
`URL = '/ueditor/';`   
- 此时Ueditor就引入成功   
    
---   
##### 修改编辑器配置（如尺寸和工具栏）    
1.直接在配置文件editor_config.js中找到相应的配置项进行修改    
2.在引入文件中进行修改，实例化时在`UE.ui.Editor()`中传入配置参数即可

