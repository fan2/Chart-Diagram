### 放大缩小
control + 鼠标滚轮  
command + 0：Actual Size  
option + command + 0：Fit to Window（AutoSize）  

### 文字如何换行？
shift + enter

### 如何设置默认字体及大小？
Preferences | General 

### 批量选择对象？
shift + 点选

可在 Alignment 中选择：

- Front/Back 图层顺序；  
- 左、右、顶、底、水平居中、垂直居中 六种对齐方式；  
- 垂直、水平 等间距；  
- 等宽、等高、等尺寸。

### 定位对象
command + E：select in Explorer  
command + D：select in Diagram  

### 显示
Editors | Styles | Format | Show

- Visibility：可见域(public,protected,private,package)  
- Namespace：命名空间(model)  
- Property：属性(in/out)  
- Type：参数类型  

### 隐藏(suppress)
Editors | Styles | Format | Suppress

- Attributes：隐藏属性  
- Operations：隐藏操作  
- Receptions  
- Literals  

### 添加参数？
右键或 Model 菜单，Add | Parameter。

- Name：参数名称。  
- Type：参数类型。  
- direction：参数属性（in,inout,out,return）。  
- defaultValue：默认值。

direction 默认为 in；return 只需 type，Name 为空。

> + func(v1: t1, out v2: t2, v3: t3 = defaultValue): rt

### 连接线无法拉直？
Line Style 默认为 Oblique（倾斜），将其风格调整为 Rectilinear（直线）或 Rounded Rectilinear。

### Model | Add Diagram 中 Flowchart Diagram 灰显无法添加？
重新启动，再添加即可。

### 打开 *.mdj 文件，左侧 Navigator(Working Diagrams) 中未显示图表？
以下两种方式，可找到图表：

- Diagram Thumbnails 中点击缩略图。  
- Model Explorer 中在对应 namespace 节点下找到 Diagram 点击。  

### 导出页中去除无效元素？
在实际绘制过程中，不小心拖进去的组件，只是 delete from view，没有 delete from model，导致有些元素不属于任何图表，Export（Print to PDF）时会导出一些残缺页面。

**解决：**

> 在 `Model Explorer` 中找到对应的 model，右键 delete from model 彻底删除。
