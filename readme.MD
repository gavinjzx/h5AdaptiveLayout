#H5头尾固定，中间自适应布局#

    兼容性：使用:before,:after伪类， 兼容性为IE8+，以及其他所有浏览器,所有移动端，如果需要IE6，7支持，不要使用:before和:after属性。在SECTION上下加5REM透明边即可。（5REM是顶和底的高度。亲可以修改成亲需要的合适的高度。）

    <b>布局原理：</b>
        顶部和底部采用position:fixed方式，header设为top:0,footer设为bottom:0<br>
        顶部和底用采用fixed方式后，会跳出文档流，所以把section的高度设为100%；但是因为顶底被遮住，需要内部添加:before和:after占位。<br>
        代码是{content:" ";display:table;height:5rem}<br>bootstrap中大量使用这段代码。如栅格布局布局系统，清除浮动时大量使用。<br>
        怎么样，是不是简单到爆？<br>
        <a href="https://github.com/gavinjzx/h5AdaptiveLayout/index.html">去gitHub查看源代码</a>
        