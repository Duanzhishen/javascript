<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
<title>无标题文档</title>
</head>

<body>
<script type="text/javascript">
	var date=new Date();
	var day=date.toLocaleString();
	var Day=date.getDay();
	var oTable = document.createElement('table');
	oTable.setAttribute("border", 1);
	oTable.setAttribute("width", 400);
	oTable.setAttribute('align', "center");
	document.body.appendChild(oTable);
	var oTbody = document.createElement('tbody');
	oTable.appendChild(oTbody);
	//获取日期
		oTbody.insertRow(0);
		oTbody.rows[0].insertCell(0);
		oTbody.rows[0].cells[0].colSpan = 7;
		oTbody.rows[0].cells[0].align="center";
		oTbody.rows[0].cells[0].appendChild(document.createTextNode(day));

		oTbody.insertRow(1);
		oTbody.rows[1].insertCell(0);
   // 今天星期几，用颜色代表
		if(Day=='0')
		{
			oTbody.rows[1].cells[0].style.backgroundColor = "blue";
		}
		oTbody.rows[1].cells[0].appendChild(document.createTextNode('星期七'));
		oTbody.rows[1].insertCell(1);
		if(Day=='1')
		{
			oTbody.rows[1].cells[1].style.backgroundColor = "blue";
		}
		oTbody.rows[1].cells[1].appendChild(document.createTextNode('星期一'));
		oTbody.rows[1].insertCell(2);
		if(Day=='2')
		{
			oTbody.rows[1].cells[2].style.backgroundColor = "blue";
		}
		oTbody.rows[1].cells[2].appendChild(document.createTextNode('星期二'));
		oTbody.rows[1].insertCell(3);
		if(Day=='3')
		{
			oTbody.rows[1].cells[3].style.backgroundColor = "blue";
		}
		oTbody.rows[1].cells[3].appendChild(document.createTextNode('星期三'));
		oTbody.rows[1].insertCell(4);
		if(Day=='4')
		{
			oTbody.rows[1].cells[4].style.backgroundColor = "blue";
		}
		oTbody.rows[1].cells[4].appendChild(document.createTextNode('星期四'));
		oTbody.rows[1].insertCell(5);
		if(Day=='5')
		{
			oTbody.rows[1].cells[5].style.backgroundColor = "blue";
		}
		oTbody.rows[1].cells[5].appendChild(document.createTextNode('星期五'));
		oTbody.rows[1].insertCell(6);
		if(Day=='6')
		{
			oTbody.rows[1].cells[6].style.backgroundColor = "blue";
		}
		oTbody.rows[1].cells[6].appendChild(document.createTextNode('星期六'));
		
		oTbody.insertRow(2);
		oTbody.rows[2].insertCell(0);
		oTbody.rows[2].cells[0].colSpan = 7;
		oTbody.rows[2].cells[0].align="center";
		var img=document.createElement('img');
    //每天图片
		if(Day=='0')
			img.setAttribute("src","images/"+7+".bmp");
		if(Day=='1')
			img.setAttribute("src","images/"+1+".bmp");
		if(Day=='2')
			img.setAttribute("src","images/"+2+".bmp");
		if(Day=='3')
			img.setAttribute("src","images/"+3+".bmp");
		if(Day=='4')
			img.setAttribute("src","images/"+4+".bmp");
		if(Day=='5')
			img.setAttribute("src","images/"+5+".bmp");
		if(Day=='6')
			img.setAttribute("src","images/"+6+".bmp");
		oTbody.rows[2].cells[0].appendChild(img);	
		
		oTbody.insertRow(3);
		oTbody.rows[3].insertCell(0);
		oTbody.rows[3].cells[0].colSpan = 7;
		oTbody.rows[3].cells[0].align="center";
    //该做些什么
		if(Day=='0')
			oTbody.rows[3].cells[0].appendChild(document.createTextNode('吃饭'));
		if(Day=='1')
			oTbody.rows[3].cells[0].appendChild(document.createTextNode('睡觉'));
		if(Day=='2')
			oTbody.rows[3].cells[0].appendChild(document.createTextNode('吃饭'));	
		if(Day=='3')
			oTbody.rows[3].cells[0].appendChild(document.createTextNode('睡觉'));
		if(Day=='4')
			oTbody.rows[3].cells[0].appendChild(document.createTextNode('吃饭'));
		if(Day=='5')
			oTbody.rows[3].cells[0].appendChild(document.createTextNode('睡觉'));
		if(Day=='6')
			oTbody.rows[3].cells[0].appendChild(document.createTextNode('吃饭'));
	
</script>
</body>
</html>
