# 欢迎使用 Setable（Smart Energetic Table）

------

**Setable（Smart Energetic Table）** 是一款轻量级的类似Excel的jquery电子表格插件。可以用JS/JSON数组、CSV文件作为数据源，实现多表头、复制、粘贴、数据格式、简单运算等基本EXCEL功能，也可作为通用JS前端表格插件。


> * 轻量级
> * 高灵活
> * 强大的
> * 类EXCEL
> * 全平台

------

## 更新
- [ ] 支持以 PDF 格式导出文稿
- [ ] 改进 Cmd 渲染算法，使用局部渲染技术提高渲染效率
- [x] 新增 Todo 列表功能
- [x] 修复 LaTex 公式渲染问题
- [x] 新增 LaTex 公式编号功能

------

## 开始使用

开始使用  开始使用  开始使用  开始使用  开始使用  开始使用  

### 1. 安装 

- [ ] 支持以 PDF 格式导出文稿
- [ ] 改进 Cmd 渲染算法，使用局部渲染技术提高渲染效率
- [x] 新增 Todo 列表功能
- [x] 修复 LaTex 公式渲染问题
- [x] 新增 LaTex 公式编号功能

### 2. 配置
```javaScript
		// Table id
		container: 'setable',
		// Width of table
		width: '100%',
		// Height of table
		height: '300px',
		// Column types and configurations
		columns: [],
		// Column header titles
		colHeaders: [],
		// Allow column sorting
		colSort: true,
		// Allow column dragging
		colDrag: true,
		// Allow column resizing
		colResize: true,
		// Allow row dragging
		rowDrag: true,
		// Allow row resizing
		rowResize: true,
		// Row height
		rowHeight: '28',
		// Minimal number of rows
		minRows: 2,
		// Minimal number of cols
		minCols: 2,
		// Minimal number of blank rows in the end
		minSpareRows: 0,
		// Minimal number of blank cols in the end
		minSpareCols: 0,
		// Allow new rows
		allowInsertRow: true,
		// Allow new columns
		allowInsertCol: true,
		// Allow row delete
		allowDeleteRow: true,
		// Allow column delete
		allowDeleteCol: true,
		// Custom context menu
		contextMenu: null,
		// Filename for download
		fileName: 'setable'
```
### 3. 高亮一段代码[^code]

```javaScript
var at = new Setable({
		container: 'excel',
		minCols: 20,
		minRows: 20,
		colHeaders: [
				['省份', '商业销量', , , , , , , , '份额', , ,],
				['', '全国商业销量', , , , '湖南中烟商业销量', , , , '湖南中烟市场份额%', , ,],
				['', '本期', '同期', '增减', '增幅%', '本期', '同期', '增减', '增幅%', '本期', '同期', '增减']
		]，
		data: data
});
```