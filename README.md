# dtg.raphael.js
放大缩小拖拽插件

使用方法

	  var options = {        //常规设置
	     width:600,           //画布宽度
		   height:500,          //画布高度
		   zoom:0.5,            //放大比例
       begin:0.3,  //
		   end:0.8,    //
		   silder:{             //操作条参数
	          	  x: 10,       //左边距
	          	  y: 10,       //上边距
	        	    width:30,   //宽度
	        	    height:200, //高度
	            }, 
	  }
	  
var tree = new DtgRaphael("tree2",options);

var pathSmall = tree2.paper.image("img/bg.png",0,0,2000,1500);
var pathSmall2 = tree2.paper.image("img/people.png",0,0,2000,1500);
var pathSmall3 = tree2.paper.image("img/gift.png",800,600,160,160);
pathSmall3.click(function(e){});

tree.bindBtnData(pathSmall).bindBtnData(pathSmall2).bindBtnData(pathSmall3).startDrag();
	  
