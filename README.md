echart
======

学习echart

官网 http://echarts.baidu.com

demo1 http://s9013.github.io/echart/app/index.html

导入echarts.js

// option
  var option = {
                    tooltip: {
                        show: true
                    },
                    legend: {
                        data:['销量']
                    },
                    xAxis : [
                        {
                            type : 'category',
                            data : ["衬衫","羊毛衫","雪纺衫","裤子","高跟鞋","袜子"]
                        }
                    ],
                    yAxis : [
                        {
                            type : 'value'
                        }
                    ],
                    series : [
                        {
                            "name":"销量",
                            "type":"bar",
                            "data":[5, 20, 40, 10, 10, 20]
                        }
                    ]
                };
  // init
  var chart = echarts.init(document.getElementById('chart'));
  
  // set option
  chart.setOption(option);