# amcharts
amcharts Demo 小例子


demo路径:amcharts/samples/*.html
 
官方API地址：https://docs.amcharts.com/3/javascriptcharts/AmChart
 
官网：https://amcharts.com

..

 
以下 是3D饼图一个小例子：


var chartData1_1 = [{

            "country": "早饭量",
            
            "value": 120,
            
            "color": "#00a7ad",
            
            "labelColor": "#ffffff"
            
        },
        
        {
            "country": "午饭量",
            "value": 120,
            "color": "#af31da",
            "labelColor": "#ffffff"
        },
        {
            "country": "晚饭量",
            "value": 120,
            "color": "#3170d9",
            "labelColor": "#ffffff"
        }];
        var chart1_1 = AmCharts.makeChart("chartdiv1_1", {
            "type": "pie",//类型
            "dataProvider": chartData1_1,//数据
            "valueField": "value",//数值
            "titleField": "country",//名称
            "labelRadius": "-40",//label偏移量
            "colorField": "color",//填充颜色
            "showFirstLabel":false,
            "labelColorField": "labelColor",//label字的颜色
            "labelText": "[[country]]",//不显示数值只显示title
            "balloonText": "",//提示框
            "depth3D": 10,//3d厚度
            "angle": 30,//3d倾斜度
            "marginTop": 10,//距离上下左右的距离
            "marginBottom": -50,
            "marginRight": -20,
            "marginLeft": -20,
        });
       
