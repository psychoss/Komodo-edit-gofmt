
/*
 *一个很简单的宏，用来帮助在Komodo中编写Go语言代码
 * A very simple Marco to help coding go code in komodo Edit
 */

//获取当前试图
//get current view
var currentView = ko.views.manager.currentView;
//获取当前加载文档
//get the document had been loaded
var doc = currentView.koDoc
//获取文件路径
// get the full path
var cwd = doc.file.path

// 一种不是很理想的确定文档类型的方法
// the lose way to check the file's type
if (cwd.indexOf(".go")!==-1) {
 
 //调用文档格式化GO文件
 // invoke gofmt to refomart the go code.
  ko.run.runEncodedCommand( window,'gofmt -s -w '+cwd+ ' '+cwd);
}
