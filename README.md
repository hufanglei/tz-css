# 选择器高级+a伪类

## 基本选择器复习

		*   通配符(通用元素选择器)  	 	            
		匹配任何元素              eg :*{margin:0;padding:0;}

		tagName(标签|元素选择器)	 	
			匹配所有标签名是tagName的元素       eg:div{ width:100px;height:40px;}

		.className(class选择器)     	       
			 匹配 所有class属性中包含className的元素   eg: .box{background:red;}

 		#IDName(id选择器)		           
			匹配所有id属性等于IDName的元素    eg:#wrap{margin:20px;}  

## 高级选择器

		E,F (多元素选择器) 	
	    	同时匹配所有E元素或F元素，E和F之间用逗号分隔
	    	eg:div,p{width:100px;height:50px;}

		E F (后代选择器)		
		    匹配所有属于E元素后代的F元素，E和F之间用空格分隔-包含子元素和孙元素
		    eg:div ul li{list-style:none;}

		E > F(子元素选择器)     
		    匹配所有E元素的直接子元素F
		    eg:div>p{color:maroon;}

		E + F(毗邻元素选择器)	
		    匹配所有紧随E元素之后的同级元素F
		    eg:li+li{color:red;}

## 属性选择器（扩展 ，挺好的）

		1.  [attr]		匹配具有attr属性的E元素
			eg: a[href]{ color:red; }
			或者直接[class]:{}
		2.  [attr=val]	匹配所有attr属性等于“val”的E元素
			eg:a[href=”www.baidu.com”]
			或者直接[class=box]:{}
		3.  [attr~=val]	匹配所有attr属性包含“val”或者等于“val”的E元素
				eg:img[src ~= ”images”]{ margin:10px;}
				或者直接[class~=box]:{} 或者 或者直接[id~=box]:{}
		4.  [attr|=val]	匹配所有attr属性以“val”整个开头或'val-'的E元素
				eg:img[alt |= buy]{color:red; }
				或者直接[class|=box]:{} 或者 或者直接[id|=box]:{}
		5.  [attr1][attr2=val]	匹配所有拥有attr1属性同时具有attr2等于'val'的元素
					eg:a[href][title=图片]{text-decoration:underline;}、
				这个的匹配条件比较苛刻，如果是title必须是只有一个

## a伪类选择器

		1.    :link		匹配所有未被点击的链接
		eg: a:link{color:green;}

		2.    :visited	匹配所有已被点击的链接
		eg: a:visited{ color:red;}

		3.    :hover	匹配鼠标悬停其上的E元素
		eg: a:hover{ text-decoration:underline;}

		4.    :active	匹配鼠标已经其上按下、还没有释放的E元素
		eg: a:active{ color:purple}  

## 伪元素选择器

			
		1.    :before	在E元素内容前面插入内容
				eg: div:before{content:””}

		2.    :after	在E元素内容后面插入内容
				eg:  p:after {content:””}
		>常用于清楚浮动等				







